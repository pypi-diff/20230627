# Comparing `tmp/hikari_crescent-0.6.1.tar.gz` & `tmp/hikari_crescent-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_crescent-0.6.1.tar", max compression
+gzip compressed data, was "hikari_crescent-0.6.2.tar", max compression
```

## Comparing `hikari_crescent-0.6.1.tar` & `hikari_crescent-0.6.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    16725 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/LICENSE
--rw-r--r--   0        0        0     6951 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/README.md
--rw-r--r--   0        0        0     1235 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/__init__.py
--rw-r--r--   0        0        0      207 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/_about.py
--rw-r--r--   0        0        0     1645 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/banner.txt
--rw-r--r--   0        0        0     8056 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/client.py
--rw-r--r--   0        0        0      531 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/__init__.py
--rw-r--r--   0        0        0     2328 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/args.py
--rw-r--r--   0        0        0     7689 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/decorators.py
--rw-r--r--   0        0        0     2560 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/groups.py
--rw-r--r--   0        0        0     1775 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/hooks.py
--rw-r--r--   0        0        0    11553 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/options.py
--rw-r--r--   0        0        0     3814 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/signature.py
--rw-r--r--   0        0        0      374 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/context/__init__.py
--rw-r--r--   0        0        0     3229 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/context/autocomplete_context.py
--rw-r--r--   0        0        0     4242 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/context/base_context.py
--rw-r--r--   0        0        0    10056 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/context/context.py
--rw-r--r--   0        0        0     2109 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/context/utils.py
--rw-r--r--   0        0        0     3122 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/errors.py
--rw-r--r--   0        0        0     2673 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/event.py
--rw-r--r--   0        0        0      642 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/exceptions.py
--rw-r--r--   0        0        0     1964 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/cooldowns/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/cooldowns/py.typed
--rw-r--r--   0        0        0     2823 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/locales/__init__.py
--rw-r--r--   0        0        0      277 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/tasks/__init__.py
--rw-r--r--   0        0        0     1697 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/tasks/cron.py
--rw-r--r--   0        0        0     1614 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/tasks/loop.py
--rw-r--r--   0        0        0        0 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/tasks/py.typed
--rw-r--r--   0        0        0     2402 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/tasks/task.py
--rw-r--r--   0        0        0      281 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/internal/__init__.py
--rw-r--r--   0        0        0     6063 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/internal/app_command.py
--rw-r--r--   0        0        0     9438 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/internal/handle_resp.py
--rw-r--r--   0        0        0      980 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/internal/includable.py
--rw-r--r--   0        0        0    16835 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/internal/registry.py
--rw-r--r--   0        0        0      945 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/locale.py
--rw-r--r--   0        0        0     1315 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/mentionable.py
--rw-r--r--   0        0        0     8975 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/plugin.py
--rw-r--r--   0        0        0        0 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/py.typed
--rw-r--r--   0        0        0     2270 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/typedefs.py
--rw-r--r--   0        0        0      317 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/utils/__init__.py
--rw-r--r--   0        0        0      236 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/utils/any_issubclass.py
--rw-r--r--   0        0        0      256 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/utils/gather_iter.py
--rw-r--r--   0        0        0      629 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/utils/options.py
--rw-r--r--   0        0        0      513 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/utils/tasks.py
--rw-r--r--   0        0        0     2570 2023-06-23 06:29:28.763278 hikari_crescent-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     8336 1970-01-01 00:00:00.000000 hikari_crescent-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-06-26 22:32:04.888412 hikari_crescent-0.6.2/LICENSE
+-rw-r--r--   0        0        0     6951 2023-06-26 22:32:04.888412 hikari_crescent-0.6.2/README.md
+-rw-r--r--   0        0        0     1210 2023-06-26 22:32:04.888412 hikari_crescent-0.6.2/crescent/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-26 22:32:04.888412 hikari_crescent-0.6.2/crescent/_about.py
+-rw-r--r--   0        0        0     1645 2023-06-26 22:32:04.888412 hikari_crescent-0.6.2/crescent/banner.txt
+-rw-r--r--   0        0        0    10718 2023-06-26 22:32:04.888412 hikari_crescent-0.6.2/crescent/client.py
+-rw-r--r--   0        0        0      531 2023-06-26 22:32:04.888412 hikari_crescent-0.6.2/crescent/commands/__init__.py
+-rw-r--r--   0        0        0     3185 2023-06-26 22:32:04.888412 hikari_crescent-0.6.2/crescent/commands/args.py
+-rw-r--r--   0        0        0    11330 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/commands/decorators.py
+-rw-r--r--   0        0        0     4270 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/commands/groups.py
+-rw-r--r--   0        0        0     2382 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/commands/hooks.py
+-rw-r--r--   0        0        0    13736 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/commands/options.py
+-rw-r--r--   0        0        0     3815 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/commands/signature.py
+-rw-r--r--   0        0        0      374 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/context/__init__.py
+-rw-r--r--   0        0        0     3229 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/context/autocomplete_context.py
+-rw-r--r--   0        0        0     4242 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/context/base_context.py
+-rw-r--r--   0        0        0    14106 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/context/context.py
+-rw-r--r--   0        0        0     2109 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/context/utils.py
+-rw-r--r--   0        0        0     4388 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/errors.py
+-rw-r--r--   0        0        0     3155 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/events.py
+-rw-r--r--   0        0        0      642 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/exceptions.py
+-rw-r--r--   0        0        0     1964 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/ext/cooldowns/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/ext/cooldowns/py.typed
+-rw-r--r--   0        0        0     2823 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/ext/locales/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/ext/tasks/__init__.py
+-rw-r--r--   0        0        0     1697 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/ext/tasks/cron.py
+-rw-r--r--   0        0        0     1614 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/ext/tasks/loop.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/ext/tasks/py.typed
+-rw-r--r--   0        0        0     2402 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/ext/tasks/task.py
+-rw-r--r--   0        0        0      281 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/internal/__init__.py
+-rw-r--r--   0        0        0     6063 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/internal/app_command.py
+-rw-r--r--   0        0        0     9438 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/internal/handle_resp.py
+-rw-r--r--   0        0        0      980 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/internal/includable.py
+-rw-r--r--   0        0        0    16835 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/internal/registry.py
+-rw-r--r--   0        0        0     1050 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/locale.py
+-rw-r--r--   0        0        0     1744 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/mentionable.py
+-rw-r--r--   0        0        0     9455 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/py.typed
+-rw-r--r--   0        0        0     2341 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/typedefs.py
+-rw-r--r--   0        0        0      317 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/utils/__init__.py
+-rw-r--r--   0        0        0      236 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/utils/any_issubclass.py
+-rw-r--r--   0        0        0      256 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/utils/gather_iter.py
+-rw-r--r--   0        0        0      629 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/utils/options.py
+-rw-r--r--   0        0        0      513 2023-06-26 22:32:04.892412 hikari_crescent-0.6.2/crescent/utils/tasks.py
+-rw-r--r--   0        0        0     2570 2023-06-26 22:32:22.705420 hikari_crescent-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     8336 1970-01-01 00:00:00.000000 hikari_crescent-0.6.2/PKG-INFO
```

### Comparing `hikari_crescent-0.6.1/LICENSE` & `hikari_crescent-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/README.md` & `hikari_crescent-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/__init__.py` & `hikari_crescent-0.6.2/crescent/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from importlib.metadata import version
 from typing import Sequence
 
 from crescent.client import *
 from crescent.commands import *
 from crescent.context import *
 from crescent.errors import *
-from crescent.event import *
+from crescent.events import *
 from crescent.exceptions import *
 from crescent.locale import *
 from crescent.mentionable import *
 from crescent.plugin import *
 from crescent.typedefs import *
 
 __version__: str = version("hikari-crescent")
@@ -49,9 +49,8 @@
     "CommandOptionsT",
     "OptionTypesT",
     "HookCallbackT",
     "AutocompleteCallbackT",
     "ClassCommandProto",
     "Plugin",
     "PluginManager",
-    "ClassCommandOption",
 )
```

### Comparing `hikari_crescent-0.6.1/crescent/banner.txt` & `hikari_crescent-0.6.2/crescent/banner.txt`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/client.py` & `hikari_crescent-0.6.2/crescent/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -53,14 +53,37 @@
 
 @runtime_checkable
 class RESTTraits(InteractionServerAware, RESTAware, Protocol):
     """The base traits crescents requires for a REST-based bot."""
 
 
 class Client:
+    """
+    The client object is a wrapper around your bot that lets you use
+    Crescent's features.
+
+    ### Example
+
+    ```python
+    import hikari
+    import crescent
+
+    bot = hikari.GatewayBot("your token")
+    client = crescent.Client(bot)
+
+    # Crescent's features can be used.
+    @client.include
+    @crescent.command
+    async def ping(ctx: crescent.Context):
+        await ctx.respong("Pong")
+
+    bot.run()
+    ```
+    """
+
     def __init__(
         self,
         app: RESTTraits | GatewayTraits,
         model: Any = None,
         *,
         tracked_guilds: Sequence[Snowflakeish] | None = None,
         default_guild: Snowflakeish | None = None,
@@ -69,14 +92,38 @@
         command_hooks: list[HookCallbackT] | None = None,
         command_after_hooks: list[HookCallbackT] | None = None,
     ):
         """
         Args:
             app:
                 The hikari bot instance.
+            model:
+                An object to store global data. This object can be accessed
+                with the `Plugin.model` property.
+
+                ### Example
+
+                ```
+                # In bot.py
+                bot = hikari.GatewayBot("your token")
+                client = crescent.Client(bot, "I am a model")
+
+                client.plugins.load("plugin")
+
+                # In plugin.py
+                plugin = crescent.Plugin()
+
+                @plugin.on_load
+                def on_load():
+                    # Print the model object that was set earlier to the console.
+                    print(plugin.model)  # prints "I am a model"
+                ```
+
+                If no model is set, the model will default to `None`.
+
             tracked_guilds:
                 The guilds to compare posted commands to. Commands will not be
                 automatically removed from guilds that aren't in this list. This should
                 be kept to as little guilds as possible to prevent rate limits.
             default_guild:
                 The guild to post application commands to by default. If this is None,
                 slash commands will be posted globally.
@@ -88,15 +135,15 @@
             command_after_hooks:
                 List of hooks to run after all commands.
         """
         self.app = app
         self.model = model
 
         if update_commands:
-            self._add_startup_callback(self.post_commands)
+            self._add_startup_callback(self._post_commands)
         self._add_startup_callback(self._on_start)
 
         if tracked_guilds is None:
             tracked_guilds = ()
 
         if default_guild and default_guild not in tracked_guilds:
             tracked_guilds = tuple(chain(tracked_guilds, (default_guild,)))
@@ -120,91 +167,129 @@
         self.default_guild: Snowflakeish | None = default_guild
 
         self._plugins = PluginManager(self)
 
         self._started = False
 
         if isinstance(app, GatewayTraits):
-            app.event_manager.subscribe(InteractionCreateEvent, self.on_interaction_event)
+            app.event_manager.subscribe(InteractionCreateEvent, self._on_interaction_event)
             return
         app.interaction_server.set_listener(
             CommandInteraction,  # pyright: ignore
-            self.on_rest_interaction,  # type: ignore
+            self._on_rest_interaction,  # type: ignore
         )
         app.interaction_server.set_listener(
             AutocompleteInteraction,  # type: ignore
-            self.on_rest_interaction,  # type: ignore
+            self._on_rest_interaction,  # type: ignore
         )
 
-    async def on_rest_interaction(
+    async def _on_rest_interaction(
         self, interaction: PartialInteraction
     ) -> InteractionResponseBuilder:
         future: Future[InteractionResponseBuilder] = get_running_loop().create_future()
         create_task(handle_resp(self, interaction, future))
         return await future
 
-    async def on_interaction_event(self, event: InteractionCreateEvent) -> None:
+    async def _on_interaction_event(self, event: InteractionCreateEvent) -> None:
         await handle_resp(self, event.interaction, None)
 
-    def post_commands(self) -> Coroutine[Any, Any, None]:
+    def _post_commands(self) -> Coroutine[Any, Any, None]:
         return self._command_handler.register_commands()
 
     @overload
     def include(self, command: INCLUDABLE) -> INCLUDABLE:
         ...
 
     @overload
     def include(self, command: None = ...) -> Callable[[INCLUDABLE], INCLUDABLE]:
         ...
 
     def include(
         self, command: INCLUDABLE | None = None
     ) -> INCLUDABLE | Callable[[INCLUDABLE], INCLUDABLE]:
+        """
+        Register an includable object, such as an event or command handler.
+
+        ### Example
+
+        ```python
+        client = crescent.Client(...)
+
+        @client.include
+        @crescent.command
+        async def ping(ctx: crescent.Context):
+            await ctx.respong("Pong")
+        ```
+        """
         if command is None:
             return self.include
 
         add_hooks(self, command)
 
         command.register_to_client(self)
 
         return command
 
     @property
     def plugins(self) -> PluginManager:
+        """
+        Return the plugin manager object. This object lets you load and unload
+        plugins. See `PluginManager` for more information.
+        """
         return self._plugins
 
     @property
     def commands(self) -> CommandHandler:
+        """
+        Return the command handler object. This object lets you access command
+        information that is not normally accessible. See `CommandHandler` for
+        more information.
+        """
         return self._command_handler
 
     async def on_crescent_command_error(
         self, exc: Exception, ctx: Context, was_handled: bool
     ) -> None:
+        """
+        This function is run when there is an error in a crescent command
+        that is not caught with any error handlers. You can inherit from this
+        class and override this function to change default error handling.
+        """
         if was_handled:
             return
         with suppress(Exception):
             await ctx.respond("An unexpected error occurred.", ephemeral=True)
         print(f"Unhandled exception occurred in the command {ctx.command}:")
         print_exception(exc.__class__, exc, exc.__traceback__)
 
     async def on_crescent_event_error(
         self, exc: Exception, event: hk_Event, was_handled: bool
     ) -> None:
+        """
+        This function is run when there is an error in a crescent event
+        that is not caught with any error handlers. You can inherit from this
+        class and override this function to change default error handling.
+        """
         if was_handled:
             return
         print(f"Unhandled exception occurred for {type(event)}:")
         print_exception(exc.__class__, exc, exc.__traceback__)
 
     async def on_crescent_autocomplete_error(
         self,
         exc: Exception,
         ctx: AutocompleteContext,
         option: AutocompleteInteractionOption,
         was_handled: bool,
     ) -> None:
+        """
+        This function is run when there is an error in an autocomplete handler
+        that is not caught with any error handlers. You can inherit from this
+        class and override this function to change default error handling.
+        """
         if was_handled:
             return
         print(
             f"Unhandled exception occurred in the autocomplete interaction for {ctx.command}"
             f" (option: {option.name}):"
         )
         print_exception(exc.__class__, exc, exc.__traceback__)
```

### Comparing `hikari_crescent-0.6.1/crescent/commands/__init__.py` & `hikari_crescent-0.6.2/crescent/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/commands/hooks.py` & `hikari_crescent-0.6.2/crescent/commands/hooks.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,18 +11,45 @@
     from crescent.typedefs import HookCallbackT
 
 __all__: Sequence[str] = ("HookResult", "hook", "add_hooks")
 
 
 @dataclass
 class HookResult:
+    """
+    An object return by hooks to provide information about what to do after
+    the hook is run.
+
+    Args:
+        exit: If true, don't run any following hooks or the command.
+    """
+
     exit: bool = False
 
 
 class hook:
+    """
+    Register a hook to a command.
+
+    ### Example
+    ```python
+    async def say_hi(ctx: crescent.Context) -> None:
+        await ctx.respond("Hello there")
+
+    @client.include
+    @crescent.hook(say_hi)
+    @crescent.command
+    async def ping(ctx: crescent.Context):
+        await ctx.respond("Pong")
+    ```
+
+    Args:
+        after: If true, run this hook after the command has completed.
+    """
+
     def __init__(self, *callbacks: HookCallbackT, after: bool = False):
         self.callbacks = callbacks
         self.after = after
 
     def __call__(self, command: Includable[AppCommandMeta]) -> Includable[AppCommandMeta]:
         for callback in self.callbacks:
             if not iscoroutinefunction(callback):
```

### Comparing `hikari_crescent-0.6.1/crescent/commands/options.py` & `hikari_crescent-0.6.2/crescent/commands/options.py`

 * *Files 16% similar despite different names*

```diff
@@ -389,23 +389,80 @@
     ...
 
 
 def option(
     option_type: type[OptionTypesT] | Sequence[type[PartialChannel]],
     description: str | LocaleBuilder = "No Description",
     *,
+    name: str | LocaleBuilder | None = None,
     default: UndefinedOr[Any] = UNDEFINED,
     choices: Sequence[tuple[str | LocaleBuilder, str | int | float]] | None = None,
     min_value: int | float | None = None,
     max_value: int | float | None = None,
     min_length: int | None = None,
     max_length: int | None = None,
-    name: str | LocaleBuilder | None = None,
     autocomplete: AutocompleteCallbackT[Any] | None = None,
 ) -> ClassCommandOption[Any]:
+    """
+    An option when declaring a command using class syntax.
+
+    ### Example
+    ```python
+    @client.include
+    @crescent.command(name="say")
+    class Say:
+        word = crescent.option(str)
+
+        async def callback(self, ctx: crescent.Context):
+            await ctx.respond(self.word)
+    ```
+
+    Args:
+        description:
+            The description for this option. Defaults to "No Description".
+        name:
+            The name to use for this option. By default, the name of the
+            property on the option the option is set to will be used for the
+            name. In the above example the name would be `word`.
+        default:
+            The default value for this option. Specifying this will make this
+            option optional.
+        choices:
+            A set of choices a user can pick from for this option. Only available
+            for `int`, `str`, and `float` option types.
+        min_value:
+            The minimum value for a number the user inputs. Only available for
+            `int` and `float` option types.
+        man_value:
+            The maximum value for a number the user inputs. Only available for
+            `int` and `float` option types.
+        min_length:
+            The minimum length for a `str` that the user inputs.
+        max_length:
+            The maximum length for a `str` that the user inputs.
+        autocomplete:
+            An autocomplete callback for this option.
+
+            ### Example
+            ```python
+            async def autocomplete_response(
+                ctx: crescent.AutocompleteContext, option: hikari.AutocompleteInteractionOption
+            ) -> list[tuple[str, str]]:
+                # Return a list of tuples of (option name, option value)
+                return [("Some Option", "1234")]
+
+            @client.include
+            @crescent.command
+            class autocomplete:
+                result = crescent.option(str, "Respond to the message", autocomplete=autocomplete_response)
+
+                async def callback(self, ctx: crescent.Context) -> None:
+                    await ctx.respond(self.result, ephemeral=True)
+            ```
+    """  # noqa: E501
     _option_type: type[OptionTypesT]
     if (
         isinstance(option_type, type)
         and issubclass(option_type, PartialChannel)
         and option_type is not PartialChannel
     ):
         option_type = cast("type[VALID_CHANNEL_TYPES]", option_type)
```

### Comparing `hikari_crescent-0.6.1/crescent/commands/signature.py` & `hikari_crescent-0.6.2/crescent/commands/signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     return args
 
 
 def _get_arg(t: type[Arg] | type[Any], metadata: Iterable[Any]) -> Any | None:
     for data in metadata:
         if isinstance(data, t):
-            return getattr(data, "payload", data)
+            return getattr(data, "_payload", data)
     return None
 
 
 def _get_origin_and_metadata(param: Parameter) -> tuple[Any, Iterable[Any]]:
     typehint = param.annotation
     origin = _unwrap_optional(typehint)
     metadata = ()
```

### Comparing `hikari_crescent-0.6.1/crescent/context/autocomplete_context.py` & `hikari_crescent-0.6.2/crescent/context/autocomplete_context.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/context/base_context.py` & `hikari_crescent-0.6.2/crescent/context/base_context.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/context/utils.py` & `hikari_crescent-0.6.2/crescent/context/utils.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/errors.py` & `hikari_crescent-0.6.2/crescent/ext/tasks/task.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,83 @@
 from __future__ import annotations
 
-from typing import Any, Awaitable, Callable, Sequence, TypeVar
+from abc import ABC, abstractmethod
+from asyncio import TimerHandle, get_running_loop
+from typing import TYPE_CHECKING, Awaitable, Callable, Sequence, TypeVar
 
-from crescent.context.utils import support_custom_context
+from crescent.client import Client
+from crescent.exceptions import CrescentException
 from crescent.internal.includable import Includable
-from crescent.typedefs import (
-    AutocompleteErrorHandlerCallbackT,
-    CommandErrorHandlerCallbackT,
-    EventErrorHandlerCallbackT,
-)
-
-__all__: Sequence[str] = ("catch_command", "catch_event", "catch_autocomplete")
-
-
-T = TypeVar("T", bound=Callable[..., Awaitable[Any]])
-
-
-def _make_catch_function(
-    error_handler_var: str, supports_custom_ctx: bool = False
-) -> Callable[[type[Exception]], Callable[[T], Includable[T]]]:
-    def func(*exceptions: type[Exception]) -> Callable[[T], Includable[T]]:
-        def app_set_hook(includable: Includable[Any]) -> None:
-            for exc in exceptions:
-                getattr(includable.client, error_handler_var).register(includable, exc)
-
-        def plugin_unload_hook(includable: Includable[Any]) -> None:
-            for exc in exceptions:
-                getattr(includable.client, error_handler_var).remove(exc)
-
-        def decorator(callback: Any) -> Includable[Any]:
-            if supports_custom_ctx:
-                maybe_supports_custom_ctx: Callable[..., Awaitable[Any]] = support_custom_context(
-                    callback
-                )
-            else:
-                maybe_supports_custom_ctx = callback
-
-            includable = Includable(
-                maybe_supports_custom_ctx,
-                client_set_hooks=[app_set_hook],
-                plugin_unload_hooks=[plugin_unload_hook],
-            )
-
-            return includable
-
-        return decorator
-
-    return func
-
-
-_catch_command = _make_catch_function("_command_error_handler", supports_custom_ctx=True)
-_catch_event = _make_catch_function("_event_error_handler")
-_catch_autocomplete = _make_catch_function("_autocomplete_error_handler", supports_custom_ctx=True)
-
-
-# NOTE: These functions are defined to help properly type the user facings functions and
-# so linters view the catch decorators as a function instead of a variable
-
-
-def catch_command(
-    *exceptions: type[Exception],
-) -> Callable[[CommandErrorHandlerCallbackT[Any]], Includable[CommandErrorHandlerCallbackT[Any]]]:
-    """
-    Catch an exception or subclasses of an exception passed into this function when the
-    exception is raised in a command.
-    """
-    return _catch_command(*exceptions)
-
-
-def catch_event(
-    *exceptions: type[Exception],
-) -> Callable[[EventErrorHandlerCallbackT[Any]], Includable[EventErrorHandlerCallbackT[Any]]]:
-    """
-    Catch an exception or subclasses of an exception passed into this function when the
-    exception is raised in an event.
-    """
-    return _catch_event(*exceptions)
-
-
-def catch_autocomplete(
-    *exceptions: type[Exception],
-) -> Callable[
-    [AutocompleteErrorHandlerCallbackT[Any]], Includable[AutocompleteErrorHandlerCallbackT[Any]]
-]:
-    """
-    Catch an exception or subclasses of an exception passed into this function when the
-    exception is raised in an autocomplete handler.
-    """
-    return _catch_autocomplete(*exceptions)
+from crescent.utils import create_task
+
+if TYPE_CHECKING:
+    from asyncio import AbstractEventLoop
+
+TaskCallbackT = Callable[[], Awaitable[None]]
+
+__all__: Sequence[str] = ("TaskCallbackT", "Task", "TaskError")
+
+
+class TaskError(CrescentException):
+    ...
+
+
+class Task(ABC):
+    def __init__(self, callback: TaskCallbackT) -> None:
+        self.event_loop: AbstractEventLoop | None = None
+        self.callback = callback
+        self.timer_handle: TimerHandle | None = None
+        self.client: Client | None = None
+
+    def start(self) -> None:
+        if self.running:
+            raise TaskError("Task is already running.")
+
+        assert self.client
+        self.client._run_future(self._start_inner())
+
+    async def _start_inner(self) -> None:
+        assert self.client is not None
+
+        self.event_loop = get_running_loop()
+        self._call_next()
+
+    def stop(self) -> None:
+        if self.timer_handle:
+            self.timer_handle.cancel()
+
+    @property
+    def running(self) -> bool:
+        if not self.timer_handle:
+            return False
+        return not self.timer_handle.cancelled()
+
+    def _call_async(self) -> None:
+        create_task(self.callback())
+        self._call_next()
+
+    def _call_next(self) -> None:
+        assert self.event_loop
+        self.timer_handle = self.event_loop.call_later(self._next_iteration(), self._call_async)
+
+    @abstractmethod
+    def _next_iteration(self) -> float:
+        """Returns how long to wait until the next iteration if a task was scheduled right now."""
+        ...
+
+    @staticmethod
+    def _link(includable: Includable[_TaskType]) -> None:
+        """Sets hooks on Includable required for Task to function properly."""
+        includable.client_set_hooks.append(_on_client_set)
+        includable.plugin_unload_hooks.append(_unload)
+
+
+_TaskType = TypeVar("_TaskType", bound=Task)
+
+
+def _on_client_set(self: Includable[_TaskType]) -> None:
+    self.metadata.client = self.client
+    self.metadata.start()
+
+
+def _unload(self: Includable[_TaskType]) -> None:
+    self.metadata.stop()
```

### Comparing `hikari_crescent-0.6.1/crescent/event.py` & `hikari_crescent-0.6.2/crescent/events.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,34 @@
 ) -> Callable[[CallbackT[Any]], Includable[CallbackT[Any]]]:
     ...
 
 
 def event(
     callback: CallbackT[Any] | None = None, /, *, event_type: type[Any] | None = None
 ) -> Callable[[CallbackT[Any]], Includable[CallbackT[Any]]] | Includable[CallbackT[Any]]:
+    """
+    Listen to an event. This function should be used instead of
+    `hikari.GatewayBot.listen` whenever possible.
+
+    ### Example
+    ```python
+    import crescent
+
+    client = crescent.Client(...)
+
+    # Listen to the message create event
+    @client.include
+    @crescent.event
+    async def ping(event: hikari.MessageCreateEvent):
+        ...
+    ```
+
+    Event types can be provided using the `event_type` kwarg if you do not want
+    to use type annotations.
+    """
     if callback is None:
         return partial(event, event_type=event_type)  # pyright: ignore
 
     if not event_type:
         event_type = next(iter(get_type_hints(callback).values()))
 
     if not event_type:
```

### Comparing `hikari_crescent-0.6.1/crescent/exceptions.py` & `hikari_crescent-0.6.2/crescent/exceptions.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/ext/cooldowns/__init__.py` & `hikari_crescent-0.6.2/crescent/ext/cooldowns/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/ext/locales/__init__.py` & `hikari_crescent-0.6.2/crescent/ext/locales/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/ext/tasks/cron.py` & `hikari_crescent-0.6.2/crescent/ext/tasks/cron.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/ext/tasks/loop.py` & `hikari_crescent-0.6.2/crescent/ext/tasks/loop.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/internal/app_command.py` & `hikari_crescent-0.6.2/crescent/internal/app_command.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/internal/handle_resp.py` & `hikari_crescent-0.6.2/crescent/internal/handle_resp.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/internal/includable.py` & `hikari_crescent-0.6.2/crescent/internal/includable.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/internal/registry.py` & `hikari_crescent-0.6.2/crescent/internal/registry.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/locale.py` & `hikari_crescent-0.6.2/crescent/locale.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 from abc import ABC, abstractmethod
 from typing import Mapping, Sequence
 
 __all__: Sequence[str] = ("LocaleBuilder", "str_or_build_locale")
 
 
 class LocaleBuilder(ABC):
+    """
+    A class that can be inherited from to created APIs to use locales in your
+    code.
+    """
+
     @abstractmethod
     def build(self) -> Mapping[str, str]:
         """
         Builds the locales for a command. Returns a `Mapping` of
         language codes to strings.
 
         [Discord API Docs Localization.](https://discord.com/developers/docs/interactions/application-commands#localization)
```

### Comparing `hikari_crescent-0.6.1/crescent/mentionable.py` & `hikari_crescent-0.6.2/crescent/mentionable.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,30 @@
     from hikari import CommandInteraction, Role, User
 
 __all__: Sequence[str] = ("Mentionable",)
 
 
 @dataclass
 class Mentionable:
+    """
+    Represent's discord's mentionable type. A mentionable can be a User or Role.
+    Not that it can not be both.
+
+    ### Example
+    ```python
+    @client.include
+    @crescent.command
+    async def command(ctx: crescent.Context, mentionable: crescent.Mentionable):
+        if mentionable.is_user:
+            user = mentionable.unwrap_user()
+        else:
+            role = mentionable.unwrap_role()
+    ```
+    """
+
     __slots__ = ("user", "role")
 
     user: User | None
     role: Role | None
 
     @classmethod
     def _from_interaction(cls: type[Mentionable], interaction: CommandInteraction) -> Mentionable:
```

### Comparing `hikari_crescent-0.6.1/crescent/plugin.py` & `hikari_crescent-0.6.2/crescent/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 ModelT = TypeVar("ModelT")
 
 
 _LOG = getLogger(__name__)
 
 
 class PluginManager:
+    """
+    A class that allows you to load and unload plugins. You should not construct
+    this class yourself. It will be provided to you as the `clients.plugins`
+    property when you construct a `Client` object.
+    """
+
     def __init__(self, client: Client) -> None:
         self.plugins: dict[str, Plugin[Any, Any]] = {}
         self._client = client
 
     @overload
     def load(self, path: str, /, *, refresh: bool = ...) -> Plugin[Any, Any]:
         ...
@@ -175,14 +181,28 @@
         Unload all of the plugins that are currently loaded.
         """
         for path in tuple(self.plugins.keys()):
             self.unload(path)
 
 
 class Plugin(Generic[BotT, ModelT]):
+    """
+    A plugin object to be used in a plugin file.
+
+    ### Example
+    ```python
+    import hikari
+    import crescent
+
+    plugin = crescent.Plugin[hikari.GatewayBot, None]()
+    ```
+
+    You can load this file with `PluginManager.load`
+    """
+
     def __init__(
         self,
         *,
         command_hooks: list[HookCallbackT] | None = None,
         command_after_hooks: list[HookCallbackT] | None = None,
     ) -> None:
         self.command_hooks = command_hooks
```

### Comparing `hikari_crescent-0.6.1/crescent/typedefs.py` & `hikari_crescent-0.6.2/crescent/typedefs.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     Awaitable[Tuple[Sequence[Tuple[str, AutocompleteValueT]], "BaseContext"]],
 ]
 
 PluginCallbackT = Callable[[], None]
 
 
 class ClassCommandProto(Protocol):
+    """A type with all the attributes required for class commands."""
+
     async def callback(self, ctx: Any) -> Any:
         ...
 
 
 ERROR = TypeVar("ERROR", bound=Exception, contravariant=True)
 
 CommandErrorHandlerCallbackT = Callable[[ERROR, Any], Awaitable[None]]
```

### Comparing `hikari_crescent-0.6.1/crescent/utils/options.py` & `hikari_crescent-0.6.2/crescent/utils/options.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/crescent/utils/tasks.py` & `hikari_crescent-0.6.2/crescent/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.1/pyproject.toml` & `hikari_crescent-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-crescent"
-version = "v0.6.1"
+version = "v0.6.2"
 description = "🌙 A command handler for Hikari that keeps your project neat and tidy."
 readme = "README.md"
 authors = ["Lunarmagpie <bambolambo0@gmail.com>"]
 maintainers = [
     "Lunarmagpie <bambolambo0@gmail.com>",
     "Circuit <circuitsacul@icloud.com>",
 ]
```

### Comparing `hikari_crescent-0.6.1/PKG-INFO` & `hikari_crescent-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-crescent
-Version: 0.6.1
+Version: 0.6.2
 Summary: 🌙 A command handler for Hikari that keeps your project neat and tidy.
 Home-page: https://github.com/hikari-crescent/hikari-crescent
 License: MPL-2.0
 Keywords: discord,hikari,command handler,slash commands,application commands
 Author: Lunarmagpie
 Author-email: bambolambo0@gmail.com
 Maintainer: Lunarmagpie
```

