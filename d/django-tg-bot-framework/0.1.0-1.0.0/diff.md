# Comparing `tmp/django_tg_bot_framework-0.1.0.tar.gz` & `tmp/django_tg_bot_framework-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tg_bot_framework-0.1.0.tar", max compression
+gzip compressed data, was "django_tg_bot_framework-1.0.0.tar", max compression
```

## Comparing `django_tg_bot_framework-0.1.0.tar` & `django_tg_bot_framework-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      380 2023-06-21 15:05:59.441296 django_tg_bot_framework-0.1.0/django_tg_bot_framework/__init__.py
--rw-r--r--   0        0        0      181 2023-06-21 15:05:59.441296 django_tg_bot_framework-0.1.0/django_tg_bot_framework/apps.py
--rw-r--r--   0        0        0      339 2023-06-21 15:05:59.441296 django_tg_bot_framework-0.1.0/django_tg_bot_framework/contextvars_tools.py
--rw-r--r--   0        0        0     1217 2023-06-21 15:05:59.442298 django_tg_bot_framework-0.1.0/django_tg_bot_framework/decorators.py
--rw-r--r--   0        0        0      118 2023-06-21 15:05:59.442899 django_tg_bot_framework-0.1.0/django_tg_bot_framework/exceptions.py
--rw-r--r--   0        0        0     5791 2023-06-21 15:05:59.442899 django_tg_bot_framework-0.1.0/django_tg_bot_framework/models.py
--rw-r--r--   0        0        0     4009 2023-06-21 15:05:59.446997 django_tg_bot_framework-0.1.0/django_tg_bot_framework/routes.py
--rw-r--r--   0        0        0     2562 2023-06-21 15:05:59.446997 django_tg_bot_framework-0.1.0/django_tg_bot_framework/state_machine.py
--rw-r--r--   0        0        0     2690 2023-06-21 15:05:59.447985 django_tg_bot_framework-0.1.0/django_tg_bot_framework/states.py
--rw-r--r--   0        0        0     1575 2023-06-21 15:05:59.452759 django_tg_bot_framework-0.1.0/django_tg_bot_framework/views.py
--rw-r--r--   0        0        0      600 2023-06-22 09:18:52.680219 django_tg_bot_framework-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      260 2023-06-21 15:05:59.440304 django_tg_bot_framework-0.1.0/README.md
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 django_tg_bot_framework-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      380 2023-06-27 19:28:18.938977 django_tg_bot_framework-1.0.0/django_tg_bot_framework/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-27 19:30:31.900662 django_tg_bot_framework-1.0.0/django_tg_bot_framework/apps.py
+-rw-r--r--   0        0        0      339 2023-06-27 19:30:32.976458 django_tg_bot_framework-1.0.0/django_tg_bot_framework/contextvars_tools.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:43:15.587650 django_tg_bot_framework-1.0.0/django_tg_bot_framework/debug_states.py
+-rw-r--r--   0        0        0     1291 2023-06-27 13:43:15.588656 django_tg_bot_framework-1.0.0/django_tg_bot_framework/decorators.py
+-rw-r--r--   0        0        0      112 2023-06-27 13:43:15.589655 django_tg_bot_framework-1.0.0/django_tg_bot_framework/exceptions.py
+-rw-r--r--   0        0        0     5676 2023-06-27 13:43:15.591655 django_tg_bot_framework-1.0.0/django_tg_bot_framework/models.py
+-rw-r--r--   0        0        0     3899 2023-06-27 13:43:15.592655 django_tg_bot_framework-1.0.0/django_tg_bot_framework/routes.py
+-rw-r--r--   0        0        0     2448 2023-06-27 13:43:15.597644 django_tg_bot_framework-1.0.0/django_tg_bot_framework/state_machine.py
+-rw-r--r--   0        0        0     2598 2023-06-27 13:43:15.595716 django_tg_bot_framework-1.0.0/django_tg_bot_framework/states.py
+-rw-r--r--   0        0        0     1527 2023-06-27 13:43:15.598739 django_tg_bot_framework-1.0.0/django_tg_bot_framework/views.py
+-rw-r--r--   0        0        0      479 2023-06-27 19:32:16.856541 django_tg_bot_framework-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7663 2023-06-27 19:28:18.936735 django_tg_bot_framework-1.0.0/README.md
+-rw-r--r--   0        0        0     8089 1970-01-01 00:00:00.000000 django_tg_bot_framework-1.0.0/PKG-INFO
```

### Comparing `django_tg_bot_framework-0.1.0/django_tg_bot_framework/decorators.py` & `django_tg_bot_framework-1.0.0/django_tg_bot_framework/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-import re
-from typing import Any, Type
-
-from tg_api import Update
-
-from .states import BaseState
-from .routes import Router, StateDecoratorType
-
-TG_COMMAND_REGEXP = re.compile(
-    r'''^
-        (?P<command>
-            /[a-zA-Z0-9_]{0,31}
-        )
-        \b
-    ''',
-    re.VERBOSE,
-)
-
-
-def select_new_state_if_command(router: Router, text: str):
-    match = TG_COMMAND_REGEXP.match(text)
-    if not match:
-        return
-
-    state_class_locator = match['command'].lower()
-
-    if not state_class_locator.endswith('/'):
-        state_class_locator = f'{state_class_locator}/'
-
-    if state_class_locator in router:
-        return router.locate(state_class_locator)
-
-
-def redirect_tg_commands(state_class: Type[BaseState]) -> StateDecoratorType:
-    class WrappedStateClass(state_class):
-        def process(self, event: Any) -> BaseState | None:
-            if isinstance(event, Update):
-                text = event.message and event.message.text or ''
-                new_state = select_new_state_if_command(self.router, text)
-                return new_state or super().process(event=event)
-            return super().process(event=event)
-    return WrappedStateClass
+import re
+from typing import Any, Type
+
+from tg_api import Update
+
+from .states import BaseState
+from .routes import Router, StateDecoratorType
+
+TG_COMMAND_REGEXP = re.compile(
+    r'''^
+        (?P<command>
+            /[a-zA-Z0-9_]{0,31}
+        )
+        \b
+    ''',
+    re.VERBOSE,
+)
+
+
+def select_new_state_if_command(router: Router, text: str):
+    match = TG_COMMAND_REGEXP.match(text)
+    if not match:
+        return
+
+    state_class_locator = match['command'].lower()
+
+    if not state_class_locator.endswith('/'):
+        state_class_locator = f'{state_class_locator}/'
+
+    if state_class_locator in router:
+        # command, *command_args = text.split()
+        # return router.locate(state_class_locator, **command_args)
+        return router.locate(state_class_locator)
+
+
+def redirect_tg_commands(state_class: Type[BaseState]) -> StateDecoratorType:
+    class WrappedStateClass(state_class):
+        def process(self, event: Any) -> BaseState | None:
+            if isinstance(event, Update):
+                text = event.message and event.message.text or ''
+                new_state = select_new_state_if_command(self.router, text)
+                return new_state or super().process(event=event)
+            return super().process(event=event)
+    return WrappedStateClass
```

### Comparing `django_tg_bot_framework-0.1.0/django_tg_bot_framework/models.py` & `django_tg_bot_framework-1.0.0/django_tg_bot_framework/models.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-import re
-import string
-
-from django.core.exceptions import ValidationError
-from django.db import models
-
-from .routes import STATE_CLASS_LOCATOR_PATTERN
-
-TG_USERNAME_PATTERN = r"^[a-zA-Z0-9_]{5,50}$"
-TG_USERNAME_INVALID_CHARS_PATTERN = r"[^a-zA-Z0-9_]"
-
-
-def validate_tg_username_friendly_to_user(value: str) -> None:
-    """Проводит ту же валидацию, что выполяет БД с помощью constraints, но генерирует понятные пользователю ошибки."""
-    if len(value) < 5:
-        raise ValidationError("Ник в телеграме должен иметь длину больше 5")
-
-    if value.startswith('@'):
-        raise ValidationError("Введите ник в телеграме без символа @.")
-
-    found_invalid_chars = re.findall(TG_USERNAME_INVALID_CHARS_PATTERN, value)
-    if found_invalid_chars:
-        invalid_chars_description = ", ".join({repr(char) for char in found_invalid_chars})
-        raise ValidationError(f"Ник в телеграмме содержит запрещённые символы: {invalid_chars_description}")
-
-
-def validate_state_class_locator_friendly_to_user(value: str) -> None:
-    """Проводит ту же валидацию, что выполяет БД с помощью constraints, но генерирует понятные пользователю ошибки."""
-    if not value.startswith('/'):
-        raise ValidationError('Локатор класса состояния должен начинаться со слэша `/`.')
-
-    if not value.endswith('/'):
-        raise ValidationError('Локатор класса состояния должен заканчиваться слэшом `/`.')
-
-    if ' ' in value:
-        raise ValidationError(
-            'Локатор класса состояния не может содержать пробелов. Используйте символы тире и подчёркивания.',
-        )
-
-    if set(value) & set(string.ascii_uppercase):
-        raise ValidationError('Локатор класса состояния содержит символы в верхнем регистре.')
-
-    allowed_symbols = f'{string.ascii_lowercase}{string.digits}_-/'
-    prohibited_symbols = set(value) - set(allowed_symbols)
-
-    if prohibited_symbols:
-        raise ValidationError(f'Локатор класса состояния содержит запрещённые символы: {prohibited_symbols!r}')
-
-
-class BaseStateMachineDump(models.Model):
-    state_class_locator = models.CharField(
-        'Класс состояния',
-        blank=True,
-        help_text='Тип состояния, в котором сейчас находится диалог с пользователем. '
-                  'В поле хранится локатор класса состояния, похожий на строку адреса URL. '
-                  'Локатор начинается со слэша <code>/</code> и заканчивается слэшом <code>/</code>, '
-                  'содержит только латинские символы a-z, цифры, знаки тире, подчёркивания и слэша <code>/</code>. '
-                  'Строго нижний регистр букв.',
-        validators=[validate_state_class_locator_friendly_to_user],
-    )
-    state_params = models.JSONField(
-        'Параметры состояния',
-        null=True,
-        blank=True,
-        help_text='Дополнительные параметры того состояния, в котором сейчас находится диалог с пользователем.',
-    )
-
-    class Meta:
-        abstract = True
-        verbose_name = "Стейт-машина"
-        verbose_name_plural = "Стейт-машины"
-        constraints = [
-            models.CheckConstraint(
-                check=models.Q(
-                    state_class_locator__regex=STATE_CLASS_LOCATOR_PATTERN) | models.Q(state_class_locator=''),
-                name="correct_state_class_locator_format",
-            ),
-        ]
-
-
-class BaseTgUser(models.Model):
-    tg_username = models.CharField(
-        "Имя юзера в Tg",
-        max_length=50,
-        blank=True,
-        db_index=True,
-        validators=[validate_tg_username_friendly_to_user],
-        help_text="Имя для поиска человека в Telegram. "
-                  "Обычно выглядит так: @username. Вводите без символа @. "
-                  "Поле может быть пустым, если у пользователя tg не указан username.",
-    )
-
-    tg_user_id = models.CharField(
-        "Id юзера в Tg",
-        max_length=50,
-        unique=True,
-        db_index=True,
-        help_text="Пример: 123456789. Чтобы узнать ID пользователя, перешлите сообщение пользователя боту "
-                  "<a href='https://t.me/userinfobot'>@userinfobot</a>.",
-    )
-
-    class Meta:
-        abstract = True
-        verbose_name = "Пользователь tg-бота"
-        verbose_name_plural = "Пользователи tg-бота"
-        constraints = [
-            models.CheckConstraint(
-                check=models.Q(tg_username__regex=TG_USERNAME_PATTERN) | models.Q(tg_username=''),
-                name="tg_username_correspond_to_spec",
-            ),
-        ]
-
-    def __str__(self):
-        tg_username_label = self.tg_username or '???'
-        return f'{tg_username_label} ({self.tg_user_id})'
+import re
+import string
+
+from django.core.exceptions import ValidationError
+from django.db import models
+
+from .routes import STATE_CLASS_LOCATOR_PATTERN
+
+TG_USERNAME_PATTERN = r"^[a-zA-Z0-9_]{5,50}$"
+TG_USERNAME_INVALID_CHARS_PATTERN = r"[^a-zA-Z0-9_]"
+
+
+def validate_tg_username_friendly_to_user(value: str) -> None:
+    """Проводит ту же валидацию, что выполяет БД с помощью constraints, но генерирует понятные пользователю ошибки."""
+    if len(value) < 5:
+        raise ValidationError("Ник в телеграме должен иметь длину больше 5")
+
+    if value.startswith('@'):
+        raise ValidationError("Введите ник в телеграме без символа @.")
+
+    found_invalid_chars = re.findall(TG_USERNAME_INVALID_CHARS_PATTERN, value)
+    if found_invalid_chars:
+        invalid_chars_description = ", ".join({repr(char) for char in found_invalid_chars})
+        raise ValidationError(f"Ник в телеграмме содержит запрещённые символы: {invalid_chars_description}")
+
+
+def validate_state_class_locator_friendly_to_user(value: str) -> None:
+    """Проводит ту же валидацию, что выполяет БД с помощью constraints, но генерирует понятные пользователю ошибки."""
+    if not value.startswith('/'):
+        raise ValidationError('Локатор класса состояния должен начинаться со слэша `/`.')
+
+    if not value.endswith('/'):
+        raise ValidationError('Локатор класса состояния должен заканчиваться слэшом `/`.')
+
+    if ' ' in value:
+        raise ValidationError(
+            'Локатор класса состояния не может содержать пробелов. Используйте символы тире и подчёркивания.',
+        )
+
+    if set(value) & set(string.ascii_uppercase):
+        raise ValidationError('Локатор класса состояния содержит символы в верхнем регистре.')
+
+    allowed_symbols = f'{string.ascii_lowercase}{string.digits}_-/'
+    prohibited_symbols = set(value) - set(allowed_symbols)
+
+    if prohibited_symbols:
+        raise ValidationError(f'Локатор класса состояния содержит запрещённые символы: {prohibited_symbols!r}')
+
+
+class BaseStateMachineDump(models.Model):
+    state_class_locator = models.CharField(
+        'Класс состояния',
+        blank=True,
+        help_text='Тип состояния, в котором сейчас находится диалог с пользователем. '
+                  'В поле хранится локатор класса состояния, похожий на строку адреса URL. '
+                  'Локатор начинается со слэша <code>/</code> и заканчивается слэшом <code>/</code>, '
+                  'содержит только латинские символы a-z, цифры, знаки тире, подчёркивания и слэша <code>/</code>. '
+                  'Строго нижний регистр букв.',
+        validators=[validate_state_class_locator_friendly_to_user],
+    )
+    state_params = models.JSONField(
+        'Параметры состояния',
+        null=True,
+        blank=True,
+        help_text='Дополнительные параметры того состояния, в котором сейчас находится диалог с пользователем.',
+    )
+
+    class Meta:
+        abstract = True
+        verbose_name = "Стейт-машина"
+        verbose_name_plural = "Стейт-машины"
+        constraints = [
+            models.CheckConstraint(
+                check=models.Q(
+                    state_class_locator__regex=STATE_CLASS_LOCATOR_PATTERN) | models.Q(state_class_locator=''),
+                name="correct_state_class_locator_format",
+            ),
+        ]
+
+
+class BaseTgUser(models.Model):
+    tg_username = models.CharField(
+        "Имя юзера в Tg",
+        max_length=50,
+        blank=True,
+        db_index=True,
+        validators=[validate_tg_username_friendly_to_user],
+        help_text="Имя для поиска человека в Telegram. "
+                  "Обычно выглядит так: @username. Вводите без символа @. "
+                  "Поле может быть пустым, если у пользователя tg не указан username.",
+    )
+
+    tg_user_id = models.CharField(
+        "Id юзера в Tg",
+        max_length=50,
+        unique=True,
+        db_index=True,
+        help_text="Пример: 123456789. Чтобы узнать ID пользователя, перешлите сообщение пользователя боту "
+                  "<a href='https://t.me/userinfobot'>@userinfobot</a>.",
+    )
+
+    class Meta:
+        abstract = True
+        verbose_name = "Пользователь tg-бота"
+        verbose_name_plural = "Пользователи tg-бота"
+        constraints = [
+            models.CheckConstraint(
+                check=models.Q(tg_username__regex=TG_USERNAME_PATTERN) | models.Q(tg_username=''),
+                name="tg_username_correspond_to_spec",
+            ),
+        ]
+
+    def __str__(self):
+        tg_username_label = self.tg_username or '???'
+        return f'{tg_username_label} ({self.tg_user_id})'
```

### Comparing `django_tg_bot_framework-0.1.0/django_tg_bot_framework/state_machine.py` & `django_tg_bot_framework-1.0.0/django_tg_bot_framework/state_machine.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from itertools import count
-import logging
-from typing import final, Any
-
-from pydantic import BaseModel, Field
-
-from .states import BaseState
-from .exceptions import TooLongTransitionError
-
-logger = logging.getLogger('django_tg_bot_framework')
-
-
-@final
-class StateMachine(BaseModel):
-    current_state: BaseState
-    max_transition_length: int = Field(
-        default=20,
-        description='Защита от зацикливания. '
-                    'Ограничивает максимальное количество непрерывных переходов между состояниями.',
-    )
-
-    def reenter_state(self, event: Any) -> None:
-        next_state = self.current_state.enter_state(event)
-        self.switch_to(next_state or self.current_state, event)
-
-    def process(self, event: Any):
-        """Обрабатывает поступившее событие."""
-        next_state = self.current_state.process(event=event)
-        self.switch_to(next_state or self.current_state, event)
-
-    def switch_to(self, next_state: BaseState, event: Any):
-        """Переключает стейт-машину в новое состояние и следует далее по авто-переходам до конечного состояния."""
-        if not isinstance(next_state, BaseState):
-            raise ValueError(f'Expect BaseState subclass as next_state value, got {next_state!r}')
-
-        counter = count(1)
-
-        if self.current_state == next_state:
-            return
-
-        prev_state = self.current_state
-
-        for transition_length in counter:
-            if transition_length > self.max_transition_length:
-                raise TooLongTransitionError(
-                    f'Transition length limit of {self.max_transition_length} is exceeded.',
-                )
-
-            logger.debug(
-                'State %s → %s.',
-                prev_state.state_class_locator,
-                next_state.state_class_locator,
-            )
-            logger.debug('    Old: %s', prev_state)
-            logger.debug('    New: %s', next_state)
-
-            state_class_transition = type(prev_state) != type(next_state)
-            prev_state.exit_state(state_class_transition=state_class_transition)
-            next_next_state = next_state.enter_state(event)
-
-            if not next_next_state:
-                break
-
-            prev_state, next_state = next_state, next_next_state
-
-        self.current_state = next_state
+from itertools import count
+import logging
+from typing import final, Any
+
+from pydantic import BaseModel, Field
+
+from .states import BaseState
+from .exceptions import TooLongTransitionError
+
+logger = logging.getLogger('django_tg_bot_framework')
+
+
+@final
+class StateMachine(BaseModel):
+    current_state: BaseState
+    max_transition_length: int = Field(
+        default=20,
+        description='Защита от зацикливания. '
+                    'Ограничивает максимальное количество непрерывных переходов между состояниями.',
+    )
+
+    def reenter_state(self) -> None:
+        next_state = self.current_state.enter_state()
+        self.switch_to(next_state or self.current_state)
+
+    def process(self, event: Any):
+        """Обрабатывает поступившее событие."""
+        next_state = self.current_state.process(event=event)
+        self.switch_to(next_state or self.current_state)
+
+    def switch_to(self, next_state: BaseState):
+        """Переключает стейт-машину в новое состояние и следует далее по авто-переходам до конечного состояния."""
+        if not isinstance(next_state, BaseState):
+            raise ValueError(f'Expect BaseState subclass as next_state value, got {next_state!r}')
+
+        counter = count(1)
+
+        if self.current_state == next_state:
+            return
+
+        prev_state = self.current_state
+
+        for transition_length in counter:
+            if transition_length > self.max_transition_length:
+                raise TooLongTransitionError(
+                    f'Transition length limit of {self.max_transition_length} is exceeded.',
+                )
+
+            logger.debug(
+                'State %s → %s.',
+                prev_state.state_class_locator,
+                next_state.state_class_locator,
+            )
+            logger.debug('    Old: %s', prev_state)
+            logger.debug('    New: %s', next_state)
+
+            state_class_transition = type(prev_state) != type(next_state)
+            prev_state.exit_state(state_class_transition=state_class_transition)
+            next_next_state = next_state.enter_state()
+
+            if not next_next_state:
+                break
+
+            prev_state, next_state = next_state, next_next_state
+
+        self.current_state = next_state
```

### Comparing `django_tg_bot_framework-0.1.0/django_tg_bot_framework/views.py` & `django_tg_bot_framework-1.0.0/django_tg_bot_framework/views.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import logging
-from typing import Callable
-
-from pydantic import ValidationError
-
-from django.db import transaction
-from django.http import JsonResponse, HttpRequest
-from django.views.decorators.csrf import csrf_exempt
-from django.views.decorators.http import require_http_methods
-
-from tg_api import Update
-
-
-logger = logging.getLogger('django_tg_bot_framework')
-
-
-@csrf_exempt
-@require_http_methods(["POST"])
-@transaction.non_atomic_requests
-def process_webhook_call(
-    request: HttpRequest,
-    *,
-    webhook_token: str,
-    process_update: Callable[[Update], None],
-) -> JsonResponse:
-    logger.debug('Telegram webhook called')
-
-    request_token = request.META.get('HTTP_X_TELEGRAM_BOT_API_SECRET_TOKEN')
-    if not request_token or request_token != webhook_token:
-        return JsonResponse({'error': 'Invalid secret token.'}, status=403)
-
-    try:
-        logger.debug('Receive JSON encoded Update object: %s', request.body)
-        update = Update.parse_raw(request.body)
-    except ValidationError as exc:
-        logger.warning('Invalid update object format: %s', exc.json())
-        return JsonResponse({
-            'error': 'Invalid update object format.',
-            'details': exc.errors(),
-        }, status=400)
-
-    try:
-        process_update(update)
-    except Exception:
-        logger.exception('Webhook call finished with error')
-
-    # Should response with status 200 always even if exception occurs to prevent bot be banned by Tg server
-    return JsonResponse({'ok': 'POST request processed.'})
+import logging
+from typing import Callable
+
+from pydantic import ValidationError
+
+from django.db import transaction
+from django.http import JsonResponse, HttpRequest
+from django.views.decorators.csrf import csrf_exempt
+from django.views.decorators.http import require_http_methods
+
+from tg_api import Update
+
+
+logger = logging.getLogger('django_tg_bot_framework')
+
+
+@csrf_exempt
+@require_http_methods(["POST"])
+@transaction.non_atomic_requests
+def process_webhook_call(
+    request: HttpRequest,
+    *,
+    webhook_token: str,
+    process_update: Callable[[Update], None],
+) -> JsonResponse:
+    logger.debug('Telegram webhook called')
+
+    request_token = request.META.get('HTTP_X_TELEGRAM_BOT_API_SECRET_TOKEN')
+    if not request_token or request_token != webhook_token:
+        return JsonResponse({'error': 'Invalid secret token.'}, status=403)
+
+    try:
+        logger.debug('Receive JSON encoded Update object: %s', request.body)
+        update = Update.parse_raw(request.body)
+    except ValidationError as exc:
+        logger.warning('Invalid update object format: %s', exc.json())
+        return JsonResponse({
+            'error': 'Invalid update object format.',
+            'details': exc.errors(),
+        }, status=400)
+
+    try:
+        process_update(update)
+    except Exception:
+        logger.exception('Webhook call finished with error')
+
+    # Should response with status 200 always even if exception occurs to prevent bot be banned by Tg server
+    return JsonResponse({'ok': 'POST request processed.'})
```

