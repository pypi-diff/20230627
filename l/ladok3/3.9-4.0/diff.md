# Comparing `tmp/ladok3-3.9.tar.gz` & `tmp/ladok3-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ladok3-3.9.tar", max compression
+gzip compressed data, was "ladok3-4.0.tar", max compression
```

## Comparing `ladok3-3.9.tar` & `ladok3-4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1155 2023-02-09 10:24:29.151703 ladok3-3.9/LICENSE
--rw-r--r--   0        0        0     6677 2022-10-25 12:52:56.416560 ladok3-3.9/README.md
--rw-r--r--   0        0        0      980 2023-02-09 10:25:13.624003 ladok3-3.9/doc/Makefile
--rw-r--r--   0        0        0      173 2022-10-25 09:48:40.909030 ladok3-3.9/doc/abstract.tex
--rw-r--r--   0        0        0     3723 2023-02-09 10:24:29.155703 ladok3-3.9/doc/ladok3.tex
--rw-r--r--   0        0        0     1160 2022-10-25 09:48:40.917030 ladok3-3.9/doc/preamble.tex
--rw-r--r--   0        0        0     3276 2022-10-25 09:54:49.529819 ladok3-3.9/makefiles/doc.mk
--rw-r--r--   0        0        0     1326 2022-10-20 12:02:01.907186 ladok3-3.9/makefiles/exam.mk
--rw-r--r--   0        0        0       66 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/haskell.mk
--rw-r--r--   0        0        0      820 2022-10-20 12:02:01.907186 ladok3-3.9/makefiles/miun.course.mk
--rw-r--r--   0        0        0     6206 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/miun.depend.mk
--rw-r--r--   0        0        0      664 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/miun.docs.mk
--rw-r--r--   0        0        0      611 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/miun.port.mk
--rw-r--r--   0        0        0      709 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/miun.pub.mk
--rw-r--r--   0        0        0     2912 2023-06-09 13:33:51.987944 ladok3-3.9/makefiles/noweb.mk
--rw-r--r--   0        0        0     2363 2023-06-09 13:33:51.611939 ladok3-3.9/makefiles/pkg.mk
--rw-r--r--   0        0        0     1225 2023-06-09 13:33:51.971944 ladok3-3.9/makefiles/portability.mk
--rw-r--r--   0        0        0     4827 2023-06-09 13:33:51.579938 ladok3-3.9/makefiles/pub.mk
--rw-r--r--   0        0        0     2321 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/results.mk
--rw-r--r--   0        0        0      421 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/subdir.mk
--rw-r--r--   0        0        0     6376 2023-06-09 13:33:51.979944 ladok3-3.9/makefiles/tex.mk
--rw-r--r--   0        0        0     2536 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/transform.mk
--rw-r--r--   0        0        0     1766 2023-06-21 18:26:12.197504 ladok3-3.9/pyproject.toml
--rw-r--r--   0        0        0       81 2022-10-25 12:52:56.440560 ladok3-3.9/src/ladok3/.gitignore
--rw-r--r--   0        0        0      557 2023-02-09 10:24:29.155703 ladok3-3.9/src/ladok3/Makefile
--rw-r--r--   0        0        0    43238 2023-02-09 19:44:21.886639 ladok3-3.9/src/ladok3/api.nw
--rw-r--r--   0        0        0    20641 2023-06-21 18:24:44.772562 ladok3-3.9/src/ladok3/cli.nw
--rw-r--r--   0        0        0    11785 2023-03-24 10:51:01.801680 ladok3-3.9/src/ladok3/data.nw
--rw-r--r--   0        0        0    50144 2023-06-08 19:44:13.018284 ladok3-3.9/src/ladok3/ladok3.nw
--rw-r--r--   0        0        0     8461 2023-06-08 20:34:03.363626 ladok3-3.9/src/ladok3/report.nw
--rw-r--r--   0        0        0     3747 2023-06-08 20:54:19.896194 ladok3-3.9/src/ladok3/student.nw
--rw-r--r--   0        0        0   180333 2023-02-09 19:28:11.895452 ladok3-3.9/src/ladok3/undoc.nw
--rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 ladok3-3.9/PKG-INFO
+-rw-r--r--   0        0        0     1155 2023-02-09 10:24:29.151703 ladok3-4.0/LICENSE
+-rw-r--r--   0        0        0     6677 2022-10-25 12:52:56.416560 ladok3-4.0/README.md
+-rw-r--r--   0        0        0      980 2023-02-09 10:25:13.624003 ladok3-4.0/doc/Makefile
+-rw-r--r--   0        0        0      173 2022-10-25 09:48:40.909030 ladok3-4.0/doc/abstract.tex
+-rw-r--r--   0        0        0     3723 2023-02-09 10:24:29.155703 ladok3-4.0/doc/ladok3.tex
+-rw-r--r--   0        0        0     1160 2022-10-25 09:48:40.917030 ladok3-4.0/doc/preamble.tex
+-rw-r--r--   0        0        0     3276 2022-10-25 09:54:49.529819 ladok3-4.0/makefiles/doc.mk
+-rw-r--r--   0        0        0     1326 2022-10-20 12:02:01.907186 ladok3-4.0/makefiles/exam.mk
+-rw-r--r--   0        0        0       66 2022-10-20 12:02:01.903186 ladok3-4.0/makefiles/haskell.mk
+-rw-r--r--   0        0        0      820 2022-10-20 12:02:01.907186 ladok3-4.0/makefiles/miun.course.mk
+-rw-r--r--   0        0        0     6206 2022-10-20 12:02:01.903186 ladok3-4.0/makefiles/miun.depend.mk
+-rw-r--r--   0        0        0      664 2022-10-20 12:02:01.903186 ladok3-4.0/makefiles/miun.docs.mk
+-rw-r--r--   0        0        0      611 2022-10-20 12:02:01.903186 ladok3-4.0/makefiles/miun.port.mk
+-rw-r--r--   0        0        0      709 2022-10-20 12:02:01.903186 ladok3-4.0/makefiles/miun.pub.mk
+-rw-r--r--   0        0        0     2912 2023-06-09 13:33:51.987944 ladok3-4.0/makefiles/noweb.mk
+-rw-r--r--   0        0        0     2363 2023-06-09 13:33:51.611939 ladok3-4.0/makefiles/pkg.mk
+-rw-r--r--   0        0        0     1225 2023-06-09 13:33:51.971944 ladok3-4.0/makefiles/portability.mk
+-rw-r--r--   0        0        0     4827 2023-06-09 13:33:51.579938 ladok3-4.0/makefiles/pub.mk
+-rw-r--r--   0        0        0     2321 2022-10-20 12:02:01.903186 ladok3-4.0/makefiles/results.mk
+-rw-r--r--   0        0        0      421 2022-10-20 12:02:01.903186 ladok3-4.0/makefiles/subdir.mk
+-rw-r--r--   0        0        0     6376 2023-06-09 13:33:51.979944 ladok3-4.0/makefiles/tex.mk
+-rw-r--r--   0        0        0     2536 2022-10-20 12:02:01.903186 ladok3-4.0/makefiles/transform.mk
+-rw-r--r--   0        0        0     1766 2023-06-27 12:09:03.992785 ladok3-4.0/pyproject.toml
+-rw-r--r--   0        0        0       81 2022-10-25 12:52:56.440560 ladok3-4.0/src/ladok3/.gitignore
+-rw-r--r--   0        0        0      557 2023-02-09 10:24:29.155703 ladok3-4.0/src/ladok3/Makefile
+-rw-r--r--   0        0        0    43304 2023-06-27 12:08:54.288682 ladok3-4.0/src/ladok3/api.nw
+-rw-r--r--   0        0        0    20641 2023-06-21 18:24:44.772562 ladok3-4.0/src/ladok3/cli.nw
+-rw-r--r--   0        0        0    11785 2023-03-24 10:51:01.801680 ladok3-4.0/src/ladok3/data.nw
+-rw-r--r--   0        0        0    50196 2023-06-27 12:08:54.288682 ladok3-4.0/src/ladok3/ladok3.nw
+-rw-r--r--   0        0        0     8920 2023-06-27 12:08:54.288682 ladok3-4.0/src/ladok3/report.nw
+-rw-r--r--   0        0        0     3747 2023-06-08 20:54:19.896194 ladok3-4.0/src/ladok3/student.nw
+-rw-r--r--   0        0        0   180333 2023-02-09 19:28:11.895452 ladok3-4.0/src/ladok3/undoc.nw
+-rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 ladok3-4.0/PKG-INFO
```

### Comparing `ladok3-3.9/LICENSE` & `ladok3-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/README.md` & `ladok3-4.0/README.md`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/doc/Makefile` & `ladok3-4.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/doc/ladok3.tex` & `ladok3-4.0/doc/ladok3.tex`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/doc/preamble.tex` & `ladok3-4.0/doc/preamble.tex`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/doc.mk` & `ladok3-4.0/makefiles/doc.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/exam.mk` & `ladok3-4.0/makefiles/exam.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/miun.course.mk` & `ladok3-4.0/makefiles/miun.course.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/miun.depend.mk` & `ladok3-4.0/makefiles/miun.depend.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/miun.docs.mk` & `ladok3-4.0/makefiles/miun.docs.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/miun.port.mk` & `ladok3-4.0/makefiles/miun.port.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/miun.pub.mk` & `ladok3-4.0/makefiles/miun.pub.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/noweb.mk` & `ladok3-4.0/makefiles/noweb.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/pkg.mk` & `ladok3-4.0/makefiles/pkg.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/portability.mk` & `ladok3-4.0/makefiles/portability.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/pub.mk` & `ladok3-4.0/makefiles/pub.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/results.mk` & `ladok3-4.0/makefiles/results.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/tex.mk` & `ladok3-4.0/makefiles/tex.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/makefiles/transform.mk` & `ladok3-4.0/makefiles/transform.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/pyproject.toml` & `ladok3-4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ladok3"
-version = "3.9"
+version = "4.0"
 description = "Python wrapper and CLI for the LADOK3 REST API."
 authors = [
   "Daniel Bosk <dbosk@kth.se>",
   "Alexander Baltatzis",
   "Gerald Q. Maguire Jr"
 ]
 license = "MIT"
```

### Comparing `ladok3-3.9/src/ladok3/Makefile` & `ladok3-4.0/src/ladok3/Makefile`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/src/ladok3/api.nw` & `ladok3-4.0/src/ladok3/api.nw`

 * *Files 0% similar despite different names*

```diff
@@ -1124,22 +1124,24 @@
 
 Finally, we can finalize the reported grade.
 If [[attestant_id]] is not [[None]], then LADOK will send a notification to 
 that person.
 (LADOK changed this API request in 2022.)
 <<LadokSession data methods>>=
 def finalize_result_JSON(self,
-    result_id, last_modified, reporter_id, attestant_ids=[]):
+    result_id, last_modified, reporter_id, attestant_ids=[],
+    others=[]):
   """Marks a result as finalized (klarmarkera)"""
   response = self.put_query(
     f"/resultat/internal/resultat/klarmarkera/{result_id}",
     {
       "Beslutsfattare": attestant_ids,
       "KlarmarkeradAvUID": reporter_id,
       "RattadAv": [],
+      "OvrigaMedverkande": "\n".join(set(others)),
       "ResultatetsSenastSparad": last_modified
     }
   )
 
   if response.status_code == requests.codes.ok:
     return response.json()
   raise Exception(response.json()["Meddelande"])
```

### Comparing `ladok3-3.9/src/ladok3/cli.nw` & `ladok3-4.0/src/ladok3/cli.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/src/ladok3/data.nw` & `ladok3-4.0/src/ladok3/data.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/src/ladok3/ladok3.nw` & `ladok3-4.0/src/ladok3/ladok3.nw`

 * *Files 0% similar despite different names*

```diff
@@ -1451,15 +1451,15 @@
       raise AttributeError("can't change already attested grade")
 
     <<set the grade for CourseResult>>
 
     self.__modified = True
     self.push()
 
-  def finalize(self, notify=False):
+  def finalize(self, graders=[], notify=False):
     """Finalizes the set grade"""
     if self.modified:
       self.push()
 
     <<finalize the grade for CourseResult>>
 
   @property
@@ -1604,16 +1604,18 @@
 
 When we finalize the result, we must know who reported the result.
 <<finalize the grade for CourseResult>>=
 reporter_id = self.ladok.user_info_JSON()["AnvandareUID"]
 
 if notify:
   response = self.ladok.finalize_result_JSON(
-    self.__results_id, self.__last_modified, reporter_id, reporter_id
+    self.__results_id, self.__last_modified, reporter_id, reporter_id,
+    others=graders
   )
 else:
   response = self.ladok.finalize_result_JSON(
-    self.__results_id, self.__last_modified, reporter_id
+    self.__results_id, self.__last_modified, reporter_id,
+    others=graders
   )
 
 self.__populate_attributes(**response)
 @
```

### Comparing `ladok3-3.9/src/ladok3/report.nw` & `ladok3-4.0/src/ladok3/report.nw`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 We want to report results from the command line.
 We need the following data for each result:
 \begin{itemize}
 \item course identifier,
 \item course component,
 \item student identifier,
 \item grade, and
-\item date\footnote{Optional, we set today's date if not present.}.
+\item date\footnote{Optional, we set today's date if not present.};
+\item grader 1,
+\item grader 2,
+\item \dots
 \end{itemize}
 
 We provide two ways to do this:
 The first is to provide positional arguments on the command line.
-The second is to not provide any positinoal argument, and in this case we read 
+The second is to not provide any positional argument, and in this case we read 
 CSV data from standard input.
 
 
 \section{The [[report]] subcommand}\label{ReportCommand}
 
 This is a subcommand is run as part of the [[ladok3.cli]] module.
 We provide a function [[add_command_options]] that adds the subcommand options 
@@ -43,15 +46,15 @@
 As mentioned above, we provide two ways of doing this.
 <<add report command arguments to report parser>>=
 one_parser = report_parser.add_argument_group(
   "one result as positional args, only date is optional")
 <<add one result group arguments>>
 many_parser = report_parser.add_argument_group(
   "many results read from standard input as CSV, columns: "
-  "course, component, student, grade, date.")
+  "course, component, student, grade, date, grader 1, ..., grader N")
 <<add many results group arguments>>
 @
 
 
 \section{Report the results}
 
 We provide two functions, one for each way of reporting the results.
@@ -64,17 +67,20 @@
 @
 
 In both cases, we want to specify whether or not the results should be 
 finalized.
 We add an option whether we want to finalize the grade for attestation by the 
 examiner.
 We add this argument outside the two groups, since it's valid for both.
+<<finalize option help>>=
+Finalize the grade (mark as ready/klarmarkera) for examiner to attest.
+Note that without this option, no graders will be registered in LADOK.
 <<add report command arguments to report parser>>=
 report_parser.add_argument("-f", "--finalize",
-  help="Finalize the grade (mark as ready/klarmarkera) for examiner to attest",
+  help="""<<finalize option help>>""",
   action="store_true",
   default=False
 )
 @
 
 
 \section{Report a result given on command line}
@@ -119,25 +125,31 @@
   help="Date on ISO format (e.g. 2021-03-18), "
     f"defaults to today's date ({datetime.date.today()})",
   type=datetime.date.fromisoformat,
   default=datetime.date.today()
 )
 @
 
+Finally, we have the list of graders.
+<<add one result group arguments>>=
+one_parser.add_argument("graders", nargs="*",
+  help="Who did the grading, give as 'Name <email@instutution.se>'.")
+@
+
 Now that we have the arguments, we can just execute the following code using 
 them.
 <<report results given in args>>=
 <<check that we got all positional arguments>>
 try:
   student = ladok.get_student(args.student_id)
   <<look up [[course]] from [[student]]>>
   <<look up [[result]] from [[course]]>>
   result.set_grade(args.grade, args.date)
   if args.finalize:
-    result.finalize()
+    result.finalize(args.graders)
 except Exception as err:
   try:
     print(f"{student}: {err}")
   except ValueError as verr:
     print(f"{verr}: {args.student_id}: {err}")
 @ The option [[args.finalize]] is already set above, so we don't need to add 
 that one here.
@@ -161,15 +173,15 @@
 
 
 \section{Report many results given in standard input}
 
 We want to read CSV data from standard input.
 <<report results given in stdin>>=
 data_reader = csv.reader(sys.stdin, delimiter=args.delimiter)
-for course_code, component_code, student_id, grade, date in data_reader:
+for course_code, component_code, student_id, grade, date, *graders in data_reader:
   <<report a result read from stdin>>
 @ We need to add an argument for the delimiter.
 <<add many results group arguments>>=
 many_parser.add_argument("-d", "--delimiter",
   default="\t",
   help="The delimiter for the CSV input; "
     "default is a tab character to be compatible with POSIX commands, "
@@ -224,18 +236,19 @@
 If it's the same, we silently ignore it.
 This is best for bulk reporting, because then we can always try to report for 
 all students.
 <<set [[grade]] to [[component]], output if verbose>>=
 if not component.attested and component.grade != grade:
   component.set_grade(grade, date)
   if args.finalize:
-    component.finalize()
+    component.finalize(graders)
   if args.verbose:
     print(f"{course_code} {student}: reported "
-      f"{component.component} = {component.grade} ({date}).")
+          f"{component.component} = {component.grade} ({date}) "
+          f"by {', '.join(graders)}.")
 elif component.grade != grade:
   print(f"{course_code} {student}: attested {component.component} "
     f"result {component.grade} ({component.date}) "
     f"is different from {grade} ({date}).")
 @
```

### Comparing `ladok3-3.9/src/ladok3/student.nw` & `ladok3-4.0/src/ladok3/student.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/src/ladok3/undoc.nw` & `ladok3-4.0/src/ladok3/undoc.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.9/PKG-INFO` & `ladok3-4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladok3
-Version: 3.9
+Version: 4.0
 Summary: Python wrapper and CLI for the LADOK3 REST API.
 Home-page: https://github.com/dbosk/ladok3
 License: MIT
 Keywords: ladok3,ladok
 Author: Daniel Bosk
 Author-email: dbosk@kth.se
 Requires-Python: >=3.8,<4.0
```

