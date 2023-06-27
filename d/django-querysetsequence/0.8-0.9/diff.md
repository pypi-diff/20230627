# Comparing `tmp/django_querysetsequence-0.8-py2.py3-none-any.whl.zip` & `tmp/django_querysetsequence-0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 21117 bytes, number of entries: 9
--rw-r--r--  2.0 unx    22394 b- defN 17-Sep-05 10:20 queryset_sequence/__init__.py
--rw-r--r--  2.0 unx     2985 b- defN 17-Apr-04 12:29 queryset_sequence/_inheritance.py
--rw-r--r--  2.0 unx     8874 b- defN 16-Oct-19 13:12 queryset_sequence/pagination.py
--rw-r--r--  2.0 unx    15301 b- defN 17-Sep-05 11:11 django_querysetsequence-0.8.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx     1281 b- defN 17-Sep-05 11:11 django_querysetsequence-0.8.dist-info/metadata.json
--rw-r--r--  2.0 unx       18 b- defN 17-Sep-05 11:11 django_querysetsequence-0.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx      110 b- defN 17-Sep-05 11:11 django_querysetsequence-0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx    16428 b- defN 17-Sep-05 11:11 django_querysetsequence-0.8.dist-info/METADATA
--rw-r--r--  2.0 unx      849 b- defN 17-Sep-05 11:11 django_querysetsequence-0.8.dist-info/RECORD
-9 files, 68240 bytes uncompressed, 19649 bytes compressed:  71.2%
+Zip file size: 24195 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    21663 b- defN 18-Aug-17 17:36 queryset_sequence/__init__.py
+-rw-r--r--  2.0 unx     8850 b- defN 18-Aug-17 17:36 queryset_sequence/pagination.py
+-rw-r--r--  2.0 unx        0 b- defN 16-Jan-07 02:20 tests/__init__.py
+-rw-r--r--  2.0 unx     1643 b- defN 17-Sep-05 14:20 tests/models.py
+-rw-r--r--  2.0 unx      846 b- defN 17-Sep-05 14:20 tests/settings.py
+-rw-r--r--  2.0 unx     9367 b- defN 18-Aug-17 17:36 tests/test_pagination.py
+-rw-r--r--  2.0 unx    42269 b- defN 18-Aug-17 17:36 tests/test_querysetsequence.py
+-rw-r--r--  2.0 unx       24 b- defN 18-Sep-20 16:17 django_querysetsequence-0.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      110 b- defN 18-Sep-20 16:17 django_querysetsequence-0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx    15735 b- defN 18-Sep-20 16:17 django_querysetsequence-0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      927 b- defN 18-Sep-20 16:17 django_querysetsequence-0.9.dist-info/RECORD
+11 files, 101434 bytes uncompressed, 22643 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -1,28 +1,34 @@
 Filename: queryset_sequence/__init__.py
 Comment: 
 
-Filename: queryset_sequence/_inheritance.py
+Filename: queryset_sequence/pagination.py
 Comment: 
 
-Filename: queryset_sequence/pagination.py
+Filename: tests/__init__.py
+Comment: 
+
+Filename: tests/models.py
+Comment: 
+
+Filename: tests/settings.py
 Comment: 
 
-Filename: django_querysetsequence-0.8.dist-info/DESCRIPTION.rst
+Filename: tests/test_pagination.py
 Comment: 
 
-Filename: django_querysetsequence-0.8.dist-info/metadata.json
+Filename: tests/test_querysetsequence.py
 Comment: 
 
-Filename: django_querysetsequence-0.8.dist-info/top_level.txt
+Filename: django_querysetsequence-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: django_querysetsequence-0.8.dist-info/WHEEL
+Filename: django_querysetsequence-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: django_querysetsequence-0.8.dist-info/METADATA
+Filename: django_querysetsequence-0.9.dist-info/METADATA
 Comment: 
 
-Filename: django_querysetsequence-0.8.dist-info/RECORD
+Filename: django_querysetsequence-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## queryset_sequence/__init__.py

```diff
@@ -1,22 +1,20 @@
+from __future__ import unicode_literals
+
+from collections import defaultdict
 import functools
-from itertools import chain, dropwhile
+from itertools import dropwhile
 from operator import __not__, attrgetter, eq, ge, gt, le, lt, mul
-import uuid
 
 from django.core.exceptions import (FieldError, MultipleObjectsReturned,
                                     ObjectDoesNotExist)
 from django.db.models.base import Model
 from django.db.models.constants import LOOKUP_SEP
-from django.db.models.query import QuerySet
-from django.db.models.sql.query import Query
 from django.utils import six
 
-from queryset_sequence._inheritance import PartialInheritanceMeta
-
 # Only export the public API for QuerySetSequence. (Note that QuerySequence and
 # QuerySetSequenceModel are considered semi-public: the APIs probably won't
 # change, but implementation is not guaranteed. Other functions/classes are
 # considered implementation details.)
 __all__ = ['QuerySetSequence']
 
 
@@ -37,227 +35,23 @@
 def cumsum(seq):
     s = 0
     for c in seq:
         s += c
         yield s
 
 
-# Bridge the Django >= 1.11 Iterable object back to the Query object being an
-# iterator.
-class SequenceIterable(object):
-    def __init__(self, queryset, *args, **kwargs):
-        self.queryset = queryset._clone()
-
-    def __iter__(self):
-        return iter(self.queryset.query)
-
-
-class QuerySequence(six.with_metaclass(PartialInheritanceMeta, Query)):
-    """
-    A Query that handles multiple QuerySets.
-
-    The API is expected to match django.db.models.sql.query.Query.
-
-    """
-    INHERITED_ATTRS = [
-        'set_empty',
-        'is_empty',
-        'set_limits',
-        'clear_limits',
-        'can_filter',
-        'add_select_related',
-    ]
-    NOT_IMPLEMENTED_ATTRS = [
-        'add_annotation',
-        'add_deferred_loading',
-        'add_distinct_fields',
-        'add_extra',
-        'add_immediate_loading',
-        'add_q',
-        'add_update_fields',
-        'clear_deferred_loading',
-        'combine',
-        'get_aggregation',
-        'get_compiler',
-        'get_meta',
-        'has_filters',
-    ]
-
-    def __init__(self, *args):
-        self._querysets = list(args)
-        # Mark each QuerySet's Model with the number of the QuerySet it is.
-        for i, qs in enumerate(self._querysets):
-            # Generate a Proxy model and then modify that to allow for the same
-            # Model to be used in multiple QuerySetSequences at once.
-            qs.model = self._get_model(qs.model)
-            # Also push this to the Query object since that holds it's own
-            # reference to QuerySet.model instead of asking the QuerySet for it.
-            qs.query.model = qs.model
-
-            # Actually set the attribute.
-            setattr(qs.model, '#', i)
-
-        # Call super to pick up a variety of properties.
-        super(QuerySequence, self).__init__(model=None)
-
-    def _get_model(self, model):
-        """Create (and return) a proxy model which subclasses the given model."""
-        model_meta = getattr(model, 'Meta', object)
-
-        class QuerySequenceModel(model):
-            class Meta(model_meta):
-                proxy = True
-                # Note that we must give an app_label or Django complains, it
-                # doesn't seem to get used, however.
-                app_label = ('queryset_sequence.%s' % uuid.uuid4()).replace('-', '')
-
-        return QuerySequenceModel
-
-    def __str__(self):
-        """Return the class-name and memory location; there's no SQL to show."""
-        return object.__str__(self)
-
-    def chain(self, *args, **kwargs):
-        obj = super(QuerySequence, self).chain(*args, **kwargs)
-
-        obj._querysets = [qs._chain() for qs in self._querysets]
-        return obj
-
-    def clone(self, *args, **kwargs):
-        obj = super(QuerySequence, self).clone(*args, **kwargs)
-
-        # Clone each QuerySet and copy it to the new object.
-        obj._querysets = [it._clone() for it in self._querysets]
-        return obj
-
-    def get_count(self, using):
-        """Request count on each sub-query."""
-        if self.is_empty():
-            return 0
-        return sum([it.count() for it in self._querysets])
-
-    def has_results(self, using):
-        """If any sub-query has a result, this is true."""
-        return any([it.exists() for it in self._querysets])
-
-    def add_ordering(self, *ordering):
-        """Propagate ordering to each QuerySet and save it for iteration."""
-        if ordering:
-            self.order_by.extend(ordering)
-
-            # Remove the ordering by QuerySet before trying to order the
-            # individual QuerySets.
-            if ordering[0].lstrip('-') == '#':
-                ordering = ordering[1:]
-
-        self._querysets = [it.order_by(*ordering) for it in self._querysets]
-
-    def clear_ordering(self, force_empty):
-        """
-        Removes any ordering settings.
-
-        Does not propagate to each QuerySet since their is no appropriate API.
-        """
-        self.order_by = []
-
-    def add_select_related(self, fields):
-        # Don't bother splitting this by field sep, etc.
-        self.select_related = fields
-
-    def __iter__(self):
-        # If this is explicitly marked as empty or there's no QuerySets, just
-        # return an empty iterator.
-        if not len(self._querysets) or self.is_empty():
-            return iter([])
-
-        # Apply any select related calls.
-        if isinstance(self.select_related, (list, tuple)):
-            self._querysets = [it.select_related(*self.select_related) for it in self._querysets]
-
-        # Reverse the ordering, if necessary. Apply this to both the individual
-        # QuerySets and the ordering of the QuerySets themselves.
-        if not self.standard_ordering:
-            self._querysets = [it.reverse() for it in self._querysets]
-            self._querysets = self._querysets[::-1]
-
-        # If order is necessary, evaluate and start feeding data back.
-        if self.order_by:
-            # If the first element of order_by is '#', this means first order by
-            # QuerySet. If it isn't this, then returned the interleaved
-            # iterator.
-            if self.order_by[0].lstrip('-') != '#':
-                return self._ordered_iterator()
-
-            # Otherwise, order by QuerySet first. Handle reversing the
-            # QuerySets, if necessary.
-            elif self.order_by[0].startswith('-'):
-                self._querysets = self._querysets[::-1]
-
-        # If there is no ordering, or the ordering is specific to each QuerySet,
-        # evaluation can be pushed off further.
-
-        # Some optimization, if there is no slicing, iterate through querysets.
-        if self.low_mark == 0 and self.high_mark is None:
-            return chain(*self._querysets)
-
-        # First trim any QuerySets based on the currently set limits!
-        counts = [0]
-        counts.extend(cumsum([it.count() for it in self._querysets]))
-
-        # TODO Do we need to work with a clone of _querysets?
-
-        # Trim the beginning of the QuerySets, if necessary.
-        start_index = 0
-        if self.low_mark is not 0:
-            # Convert a negative index into a positive.
-            if self.low_mark < 0:
-                self.low_mark += counts[-1]
-
-            # Find the point when low_mark crosses a threshold.
-            for i, offset in enumerate(counts):
-                if offset <= self.low_mark:
-                    start_index = i
-                if self.low_mark < offset:
-                    break
-
-        # Trim the end of the QuerySets, if necessary.
-        end_index = len(self._querysets)
-        if self.high_mark is None:
-            # If it was unset (meaning all), set it to the maximum.
-            self.high_mark = counts[-1]
-        elif self.high_mark:
-            # Convert a negative index into a positive.
-            if self.high_mark < 0:
-                self.high_mark += counts[-1]
-
-            # Find the point when high_mark crosses a threshold.
-            for i, offset in enumerate(counts):
-                if self.high_mark <= offset:
-                    end_index = i
-                    break
-
-        # Remove iterables we don't care about.
-        self._querysets = self._querysets[start_index:end_index]
-
-        # The low_mark needs the removed QuerySets subtracted from it.
-        self.low_mark -= counts[start_index]
-        # The high_mark needs the count of all QuerySets before it subtracted
-        # from it.
-        self.high_mark -= counts[end_index - 1]
-
-        # Some optimization, if there is only one QuerySet, iterate through it.
-        if len(self._querysets) == 1:
-            return iter(self._querysets[0][self.low_mark:self.high_mark])
-
-        # Apply the offsets to the edge QuerySets.
-        self._querysets[0] = self._querysets[0][self.low_mark:]
-        self._querysets[-1] = self._querysets[-1][:self.high_mark]
-
-        # For anything left, just chain the QuerySets together.
-        return chain(*self._querysets)
+class QuerySequenceIterable(object):
+    def __init__(self, querysetsequence):
+        # Create a clone so that subsequent calls to iterate are kept separate.
+        self._querysets = querysetsequence._querysets
+        self._queryset_idxs = querysetsequence._queryset_idxs
+        self._order_by = querysetsequence._order_by
+        self._standard_ordering = querysetsequence._standard_ordering
+        self._low_mark = querysetsequence._low_mark
+        self._high_mark = querysetsequence._high_mark
 
     @classmethod
     def _get_field_names(cls, model):
         """Return a list of field names that are part of a model."""
         return [f.name for f in model._meta.get_fields()]
 
     @classmethod
@@ -333,215 +127,286 @@
             except StopIteration:
                 # Everything was equivalent.
                 return 0
 
         return comparator
 
     def _ordered_iterator(self):
-        """An iterator that takes into account the requested ordering."""
-
-        # A mapping of iterable to the current item in that iterable. (Remember
-        # that each QuerySet is already sorted.)
-        not_empty_qss = [iter(it) for it in self._querysets if it]
-        values = {it: next(it) for it in not_empty_qss}
+        """
+        Interleave the values of each QuerySet in order to handle the requested
+        ordering. Also adds the '#' property to each returned item.
+        """
+        # A list of tuples, each with:
+        #   * The iterable
+        #   * The QuerySet number
+        #   * The next value
+        #
+        # (Remember that each QuerySet is already sorted.)
+        iterables = []
+        for i, qs in zip(self._queryset_idxs, self._querysets):
+            it = iter(qs)
+            try:
+                value = next(it)
+            except StopIteration:
+                # If this is already empty, just skip it.
+                continue
+            # Set the QuerySet number so that the comparison works properly.
+            setattr(value, '#', i)
+            iterables.append((it, i, value))
 
         # The offset of items returned.
         index = 0
 
         # Create a comparison function based on the requested ordering.
-        _comparator = self._generate_comparator(self.order_by)
-        def comparator(i1, i2):
-            # Actually compare the 2nd element in each tuple, the 1st element is
-            # the generator.
-            return _comparator(i1[1], i2[1])
+        _comparator = self._generate_comparator(self._order_by)
+        def comparator(tuple_1, tuple_2):
+            # The last element in each tuple is the actual item to compare.
+            return _comparator(tuple_1[2], tuple_2[2])
         comparator = functools.cmp_to_key(comparator)
 
         # If in reverse mode, get the last value instead of the first value from
         # ordered_values below.
-        if self.standard_ordering:
+        if self._standard_ordering:
             next_value_ind = 0
         else:
             next_value_ind = -1
 
-        # Iterate until all the values are gone.
-        while values:
+        # Continue until all iterables are empty.
+        while iterables:
             # If there's only one iterator left, don't bother sorting.
-            if len(values) > 1:
+            if len(iterables) > 1:
                 # Sort the current values for each iterable.
-                ordered_values = sorted(values.items(), key=comparator)
+                iterables = sorted(iterables, key=comparator)
 
                 # The next ordering item is in the first position, unless we're
                 # in reverse mode.
-                qss, value = ordered_values.pop(next_value_ind)
+                it, i, value = iterables[next_value_ind]
             else:
-                qss, value = list(values.items())[0]
+                it, i, value = iterables[0]
 
-            # Return it if we're within the slice of interest.
-            if self.low_mark <= index:
+            # Return the next value if we're within the slice of interest.
+            if self._low_mark <= index:
                 yield value
             index += 1
             # We've left the slice of interest, we're done.
-            if index == self.high_mark:
+            if index == self._high_mark:
                 return
 
             # Iterate the iterable that just lost a value.
             try:
-                values[qss] = next(qss)
+                value = next(it)
+                # Set the QuerySet number so that the comparison works properly.
+                setattr(value, '#', i)
+                iterables[next_value_ind] = it, i, value
             except StopIteration:
                 # This iterator is done, remove it.
-                del values[qss]
+                del iterables[next_value_ind]
 
+    def _unordered_iterator(self):
+        """
+        Return the value of each QuerySet, but also add the '#' property to each
+        return item.
+        """
+        for i, qs in zip(self._queryset_idxs, self._querysets):
+            for item in qs:
+                setattr(item, '#', i)
+                yield item
 
-# TODO Inherit from django.db.models.base.Model.
-class QuerySetSequenceModel(object):
-    """
-    A fake Model that is used to throw DoesNotExist exceptions for
-    QuerySetSequence.
-    """
-    class DoesNotExist(ObjectDoesNotExist):
-        pass
+    def __iter__(self):
+        # If there's no QuerySets, just return an empty iterator.
+        if not len(self._querysets):
+            return iter([])
 
-    class MultipleObjectsReturned(MultipleObjectsReturned):
-        pass
+        # If order is necessary, evaluate and start feeding data back.
+        if self._order_by:
+            # If the first element of order_by is '#', this means first order by
+            # QuerySet. If it isn't this, then returned the interleaved
+            # iterator.
+            if self._order_by[0].lstrip('-') != '#':
+                return self._ordered_iterator()
 
-    class _meta:
-        app_label = 'queryset_sequence'
-        object_name = 'QuerySetSequenceModel'
+            # Otherwise, order by QuerySet first. Handle reversing the
+            # QuerySets, if necessary.
+            elif self._order_by[0].startswith('-'):
+                self._querysets = self._querysets[::-1]
+
+        # If there is no ordering, or the ordering is specific to each QuerySet,
+        # evaluation can be pushed off further.
+
+        # If there is no slicing, iterate through each QuerySet. This avoids
+        # calling count() on each QuerySet.
+        if self._low_mark == 0 and self._high_mark is None:
+            return self._unordered_iterator()
+
+        # First trim any QuerySets based on the currently set limits!
+        counts = [0]
+        counts.extend(cumsum([it.count() for it in self._querysets]))
+
+        # Trim the beginning of the QuerySets, if necessary.
+        start_index = 0
+        low_mark, high_mark = self._low_mark, self._high_mark
+        if low_mark is not 0:
+            # Convert a negative index into a positive.
+            if low_mark < 0:
+                low_mark += counts[-1]
+
+            # Find the point when low_mark crosses a threshold.
+            for i, offset in enumerate(counts):
+                if offset <= low_mark:
+                    start_index = i
+                if low_mark < offset:
+                    break
+
+        # Trim the end of the QuerySets, if necessary.
+        end_index = len(self._querysets)
+        if high_mark is None:
+            # If it was unset (meaning all), set it to the maximum.
+            high_mark = counts[-1]
+        elif high_mark:
+            # Convert a negative index into a positive.
+            if high_mark < 0:
+                high_mark += counts[-1]
+
+            # Find the point when high_mark crosses a threshold.
+            for i, offset in enumerate(counts):
+                if high_mark <= offset:
+                    end_index = i
+                    break
 
+        # Remove QuerySets we don't care about.
+        self._querysets = self._querysets[start_index:end_index]
+        self._queryset_idxs = self._queryset_idxs[start_index:end_index]
 
-class QuerySetSequence(six.with_metaclass(PartialInheritanceMeta, QuerySet)):
+        # The low_mark needs the removed QuerySets subtracted from it.
+        low_mark -= counts[start_index]
+        # The high_mark needs the count of all QuerySets before it subtracted
+        # from it.
+        high_mark -= counts[end_index - 1]
+
+        # Apply the offsets to the edge QuerySets (apply the high mark first
+        # in-case there's only a single QuerySet left).
+        self._querysets[-1] = self._querysets[-1][:high_mark]
+        self._querysets[0] = self._querysets[0][low_mark:]
+
+        # For anything left, just iterate through each QuerySet.
+        return self._unordered_iterator()
+
+
+class QuerySetSequence(object):
     """
     Wrapper for multiple QuerySets without the restriction on the identity of
     the base models.
 
     """
-    INHERITED_ATTRS = [
-        # Public methods that return QuerySets.
-        'filter',
-        'exclude',
-        'order_by',
-        'reverse',
-        'none',
-        'all',
-        'select_related',
-
-        # Public methods that don't return QuerySets.
-        'get',
-        'count',
-        'as_manager',
-        'exists',
-
-        # Public introspection attributes.
-        'ordered',
-        'db',
-
-        # Private methods.
-        '_chain',
-        '_clone',
-        '_fetch_all',
-        '_merge_sanity_check',
-        '_prepare',
-    ]
-    NOT_IMPLEMENTED_ATTRS = [
-        # Public methods that return QuerySets.
-        'annotate',
-        'distinct',
-        'values',
-        'values_list',
-        'dates',
-        'datetimes',
-        'extra',
-        'defer',
-        'only',
-        'using',
-        'select_for_update',
-        'raw',
-        # Public methods that don't return QuerySets.
-        'latest',
-        'earliest',
-        'first',
-        'last',
-        'aggregate',
-
-        # Public methods that don't return QuerySets. These don't make sense in
-        # the context of a QuerySetSequence.
-        'create',
-        'get_or_create',
-        'update_or_create',
-        'bulk_create',
-        'in_bulk',
-        'update',
-    ]
-
-    def __init__(self, *args, **kwargs):
-        # Create the QuerySequence object where most of the magic happens.
-        if 'query' not in kwargs:
-            kwargs['query'] = QuerySequence(*args)
-        elif args:
-            raise ValueError(
-                "Cannot provide args and a 'query' keyword argument.")
-
-        # If a particular Model class is not provided, just use the generic
-        # model class.
-        # TODO Dynamically generate the fields available in this model via
-        # introspection of the input QuerySets.
-        if 'model' not in kwargs:
-            kwargs['model'] = QuerySetSequenceModel
-
-        super(QuerySetSequence, self).__init__(**kwargs)
-
-        # Override the iterator that will be used. (Currently used only in
-        # Django >= 1.11.)
-        self._iterable_class = SequenceIterable
 
-    def iterator(self):
-        # Create a clone so that each call re-evaluates the QuerySets.
-        return self.query.clone()
+    def __init__(self, *args):
+        self._querysets = list(args)
+        # The original ordering of the QuerySets.
+        self._queryset_idxs = list(range(len(self._querysets)))
+        # Some information necessary for properly iterating through a QuerySet.
+        self._order_by = []
+        self._standard_ordering = True
+        self._low_mark, self._high_mark = 0, None
 
-    def _filter_or_exclude(self, negate, *args, **kwargs):
-        """
-        Maps _filter_or_exclude over QuerySet items and simplifies the result.
+        self._iterable_class = QuerySequenceIterable
+        self._result_cache = None
 
-        Returns QuerySetSequence, or QuerySet depending on the contents of
-        items, i.e. at least two non empty QuerySets, or exactly one non empty
-        QuerySet.
-        """
-        if args or kwargs:
-            assert self.query.can_filter(), \
-                "Cannot filter a query once a slice has been taken."
-        clone = self._clone()
+    def _clone(self):
+        clone = QuerySetSequence(*[qs._clone() for qs in self._querysets])
+        clone._queryset_idxs = self._queryset_idxs
+        clone._order_by = self._order_by
+        clone._standard_ordering = self._standard_ordering
+        clone._low_mark = self._low_mark
+        clone._high_mark = self._high_mark
 
-        # Separate the kwargs into ones that deal with QuerySets (i.e. are
-        # handled by QuerySetSequence) and ones that will be passed onto each
-        # QuerySet.
-        sequence_kwargs = {}
-        queryset_kwargs = {}
-        for kwarg, value in kwargs.items():
-            if kwarg.startswith('#'):
-                sequence_kwargs[kwarg] = value
-            else:
-                queryset_kwargs[kwarg] = value
-        clone._filter_or_exclude_querysets(negate, **sequence_kwargs)
+        return clone
 
-        # Apply the _filter_or_exclude to each QuerySet in the QuerySequence.
-        querysets = \
-            [qs._filter_or_exclude(negate, *args, **queryset_kwargs) for qs in clone.query._querysets]
+    def _fetch_all(self):
+        if self._result_cache is None:
+            self._result_cache = list(self._iterable_class(self))
+
+    # Python magic methods.
+
+    def __len__(self):
+        self._fetch_all()
+        return len(self._result_cache)
 
-        clone.query._querysets = querysets
-        return clone
+    def __iter__(self):
+        self._fetch_all()
+        return iter(self._result_cache)
 
-    def _filter_or_exclude_querysets(self, negate, **kwargs):
-        """
-        Similar to _filter_or_exclude, but run over the QuerySets in the
-        QuerySetSequence instead of over each QuerySet's fields.
+    def __bool__(self):
+        self._fetch_all()
+        return bool(self._result_cache)
 
+    def __nonzero__(self):      # Python 2 compatibility
+        return type(self).__bool__(self)
+
+    def __getitem__(self, k):
+        """
+        Retrieves an item or slice from the set of results.
         """
-        # Start with all QuerySets.
-        querysets = list(range(len(self.query._querysets)))
+        if not isinstance(k, (slice,) + six.integer_types):
+            raise TypeError
+        assert ((not isinstance(k, slice) and (k >= 0)) or
+                (isinstance(k, slice) and (k.start is None or k.start >= 0) and
+                 (k.stop is None or k.stop >= 0))), \
+            "Negative indexing is not supported."
+
+        if isinstance(k, slice):
+            qs = self._clone()
+            # If start is not given, it is 0.
+            if k.start is not None:
+                start = int(k.start)
+            else:
+                start = 0
+            # Apply the new start to any previous slices.
+            qs._low_mark += start
+
+            # If stop is not given, don't modify the stop.
+            if k.stop is not None:
+                stop = int(k.stop)
+
+                # The high mark needs to take into an account any previous
+                # offsets of the low mark.
+                offset = stop - start
+                qs._high_mark = qs._low_mark + offset
+            return list(qs)[::k.step] if k.step else qs
+
+        qs = self._clone()
+        qs._low_mark += k
+        qs._high_mark = qs._low_mark + 1
+        return list(qs)[0]
+
+    def _separate_filter_fields(self, **kwargs):
+        qss_fields, std_fields = self._separate_fields(*kwargs.keys())
+
+        # Remove any fields that start with '#' from kwargs.
+        qss_kwargs = {field: value for field, value in kwargs.items() if field in qss_fields}
+        std_kwargs = {field: value for field, value in kwargs.items() if field in std_fields}
+
+        return qss_kwargs, std_kwargs
+
+    def _separate_fields(self, *fields):
+        # Remove any fields that start with '#' from kwargs.
+        qss_fields = []
+        std_fields = []
+        for field in fields:
+            if field.startswith('#') or field.startswith('-#'):
+                qss_fields.append(field)
+            else:
+                std_fields.append(field)
 
+        return qss_fields, std_fields
+
+    def _filter_or_exclude_querysets(self, negate, **kwargs):
+        """
+        Similar to QuerySet._filter_or_exclude, but run over the QuerySets in
+        the QuerySetSequence instead of over each QuerySet's fields.
+        """
         # Ensure negate is a boolean.
         negate = bool(negate)
 
         for kwarg, value in kwargs.items():
             parts = kwarg.split(LOOKUP_SEP)
 
             # Ensure this is being used to filter QuerySets.
@@ -574,61 +439,160 @@
 
                 # These expect integers, this matches the logic in
                 # IntegerField.get_prep_value(). (Essentially treat the '#'
                 # field as an IntegerField.)
                 if value is not None:
                     value = int(value)
 
-                querysets = filter(lambda i: operator(i, value) != negate, querysets)
+                self._queryset_idxs = filter(lambda i: operator(i, value) != negate, self._queryset_idxs)
                 continue
             except KeyError:
                 # It wasn't one of the above operators, keep trying.
                 pass
 
             # Some of these seem to get handled as bytes.
             if lookup in ('contains', 'icontains'):
                 value = six.text_type(value)
-                querysets = filter(lambda i: (value in six.text_type(i)) != negate, querysets)
+                self._queryset_idxs = filter(lambda i: (value in six.text_type(i)) != negate, self._queryset_idxs)
 
             elif lookup == 'in':
-                querysets = filter(lambda i: (i in value) != negate, querysets)
+                self._queryset_idxs = filter(lambda i: (i in value) != negate, self._queryset_idxs)
 
             elif lookup in ('startswith', 'istartswith'):
                 value = six.text_type(value)
-                querysets = filter(lambda i: six.text_type(i).startswith(value) != negate, querysets)
+                self._queryset_idxs = filter(lambda i: six.text_type(i).startswith(value) != negate, self._queryset_idxs)
 
             elif lookup in ('endswith', 'iendswith'):
                 value = six.text_type(value)
-                querysets = filter(lambda i: six.text_type(i).endswith(value) != negate, querysets)
+                self._queryset_idxs = filter(lambda i: six.text_type(i).endswith(value) != negate, self._queryset_idxs)
 
             elif lookup == 'range':
                 # Inclusive include.
                 start, end = value
-                querysets = filter(lambda i: (start <= i <= end) != negate, querysets)
+                self._queryset_idxs = filter(lambda i: (start <= i <= end) != negate, self._queryset_idxs)
 
             else:
                 # Any other field lookup is not supported, e.g. date, year, month,
                 # day, week_day, hour, minute, second, isnull, search, regex, and
                 # iregex.
                 raise ValueError("Unsupported lookup '%s'" % lookup)
 
-            # Keep querysets a list in Python 3.
-            querysets = list(querysets)
+        # Convert back to a list on Python 3.
+        self._queryset_idxs = list(self._queryset_idxs)
 
-        # Finally, trim down the actual QuerySets we care about!
-        self.query._querysets = [self.query._querysets[i] for i in querysets]
+        # Finally, keep only the QuerySets we care about!
+        self._querysets = [self._querysets[i] for i in self._queryset_idxs]
 
-    def delete(self):
-        # Propagate delete to each sub-query.
-        for qs in self.query._querysets:
-            qs.delete()
+    # Methods that return new QuerySets
+    def filter(self, **kwargs):
+        qss_fields, fields = self._separate_filter_fields(**kwargs)
 
-        # Clear the result cache, in case this QuerySet gets reused.
-        self._result_cache = None
+        clone = self._clone()
+        clone._filter_or_exclude_querysets(False, **qss_fields)
+        clone._querysets = [qs.filter(**fields) for qs in clone._querysets]
+        return clone
+
+    def exclude(self, **kwargs):
+        qss_fields, fields = self._separate_filter_fields(**kwargs)
+
+        clone = self._clone()
+        clone._filter_or_exclude_querysets(True, **qss_fields)
+        clone._querysets = [qs.exclude(**fields) for qs in clone._querysets]
+        return clone
+
+    def order_by(self, *fields):
+        _, filtered_fields = self._separate_fields(*fields)
+
+        # Apply the filtered fields to each underlying QuerySet.
+        clone = self._clone()
+        clone._querysets = [qs.order_by(*filtered_fields) for qs in self._querysets]
+
+        # But keep the original fields for the clone.
+        clone._order_by = list(fields)
+        return clone
+
+    def reverse(self):
+        clone = self._clone()
+        clone._querysets = [qs.reverse() for qs in reversed(self._querysets)]
+        clone._standard_ordering = not self._standard_ordering
+        return clone
+
+    def none(self):
+        # This is a bit odd, but use the first QuerySet to properly return an
+        # that is an instance of EmptyQuerySet.
+        return self._querysets[0].none()
+
+    def all(self):
+        clone = self._clone()
+        clone._querysets = [qs.all() for qs in self._querysets]
+        return clone
+
+    def select_related(self, *fields):
+        clone = self._clone()
+        clone._querysets = [qs.select_related(*fields) for qs in self._querysets]
+        return clone
 
     def prefetch_related(self, *lookups):
-        # Don't modify self._prefetch_related_lookups, as that will cause
-        # issues, but call prefetch_related on underlying QuerySets.
         clone = self._clone()
-        clone.query._querysets = [
-            qs.prefetch_related(*lookups) for qs in clone.query._querysets]
+        clone._querysets = [qs.prefetch_related(*lookups) for qs in self._querysets]
         return clone
+
+    # Methods that do not return QuerySets
+    def get(self, **kwargs):
+        clone = self.filter(**kwargs)
+
+        result = None
+        for qs in clone._querysets:
+            try:
+                obj = qs.get()
+            except ObjectDoesNotExist:
+                pass
+            # Don't catch the MultipleObjectsReturned(), allow it to raise.
+            else:
+                # If a second object is found, raise an exception.
+                if result:
+                    raise MultipleObjectsReturned()
+                result = obj
+
+        # Checked all QuerySets and no object was found.
+        if result is None:
+            raise ObjectDoesNotExist()
+
+        # Return the only result found.
+        return result
+
+    def count(self):
+        return sum(qs.count() for qs in self._querysets) - self._low_mark
+
+    def iterator(self):
+        clone = self._clone()
+        clone._querysets = [qs.iterator() for qs in self._querysets]
+        return clone
+
+    def exists(self):
+        return any(qs.exists() for qs in self._querysets)
+
+    def delete(self):
+        deleted_count = 0
+        deleted_objects = defaultdict(int)
+        for qs in self._querysets:
+            # Delete this QuerySet.
+            current_deleted_count, current_deleted_objects = qs.delete()
+
+            # Combine the results.
+            deleted_count += current_deleted_count
+            for obj, count in current_deleted_objects.items():
+                deleted_objects[obj] += count
+
+        return deleted_count, dict(deleted_objects)
+
+    def as_manager(self):
+        pass
+
+    # Public attributes
+    @property
+    def ordered(self):
+        """
+        Returns True if the QuerySet is ordered -- i.e. has an order_by()
+        clause.
+        """
+        return bool(self._order_by)
```

## queryset_sequence/pagination.py

```diff
@@ -89,27 +89,27 @@
                 # entire QuerySetSequence.
                 if order_attr == '#':
                     queryset = queryset.filter(**kwargs)
 
                 # If there *are* QuerySets, filter just the edge QuerySet. This
                 # avoids trimming items in subsequent QuerySets that are still
                 # valid.
-                elif queryset.query._querysets:
+                elif queryset._querysets:
                     queryset = queryset._clone()
 
                     # Make a copy of the current QuerySets.
-                    querysets = queryset.query._querysets
+                    querysets = queryset._querysets
                     # Handle whether to look at the front edge or back edge of
                     # the QuerySets based on the order of iteration.
                     if self.cursor.reverse != is_reversed:
-                        queryset.query._querysets = (
+                        queryset._querysets = (
                             querysets[:-1] +
                             [querysets[-1].filter(**kwargs)])
                     else:
-                        queryset.query._querysets = (
+                        queryset._querysets = (
                             [querysets[0].filter(**kwargs)] +
                             querysets[1:])
 
         # If we have an offset cursor then offset the entire page by that amount.
         # We also always fetch an extra item in order to determine if there is a
         # page following on from this one.
         results = list(queryset[offset:offset + self.page_size + 1])
```

## Comparing `django_querysetsequence-0.8.dist-info/DESCRIPTION.rst` & `django_querysetsequence-0.9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: django-querysetsequence
+Version: 0.9
+Summary: Chain together multiple (disparate) QuerySets to treat them as a single QuerySet.
+Home-page: https://github.com/percipient/django-querysetsequence
+Author: Percipient Networks, LLC
+Author-email: support@strongarm.io
+License: ISC
+Download-URL: https://github.com/percipient/django-querysetsequence
+Keywords: django,queryset,chain,multi,multiple,iterable
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Environment :: Web Environment
+Classifier: Topic :: Internet
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Framework :: Django
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Requires-Dist: django (>=1.11)
+
 Django QuerySetSequence
 #######################
 
 .. image:: https://travis-ci.org/percipient/django-querysetsequence.svg?branch=master
     :target: https://travis-ci.org/percipient/django-querysetsequence
 
 .. image:: https://coveralls.io/repos/github/percipient/django-querysetsequence/badge.svg?branch=master
@@ -289,51 +314,18 @@
             * ``iendswith``
             * ``range``
 
 Requirements
 ============
 
 * Python (2.7, 3.4, 3.5, 3.6)
-* Django (1.8, 1.9, 1.10, 1.11)
-* (Optionally) Django REST Framework (3.2, 3.3, 3.4, 3.5, 3.6)
-
-.. list-table:: ``QuerySetSequence`` versions with support for Django/Django REST Framework
-    :header-rows: 1
-    :stub-columns: 1
+* Django (1.11, 2.0)
+* (Optionally) `Django REST Framework`_ (3.4, 3.5, 3.6, 3.7)
 
-    * -
-      - Django 1.8
-      - Django 1.9
-      - Django 1.10
-      - Django 1.11
-    * - Django REST Framework 3.2
-      - 0.7
-      - |xmark|
-      - |xmark|
-      - |xmark|
-    * - Django REST Framework 3.3
-      - 0.7
-      - 0.7
-      - |xmark|
-      - |xmark|
-    * - Django REST Framework 3.4
-      - 0.7
-      - 0.7
-      - 0.7
-      - 0.7.1
-    * - Django REST Framework 3.5
-      - 0.7.1
-      - 0.7.1
-      - 0.7.1
-      - 0.7.1
-    * - Django REST Framework 3.6
-      - 0.8
-      - 0.8
-      - 0.8
-      - 0.8
+.. _Django REST Framework: http://www.django-rest-framework.org/
 
 Installation
 ============
 
 Install the package using pip.
 
 .. code-block:: bash
```

