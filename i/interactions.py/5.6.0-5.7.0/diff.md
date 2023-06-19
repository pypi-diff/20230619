# Comparing `tmp/interactions.py-5.6.0.tar.gz` & `tmp/interactions.py-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactions.py-5.6.0.tar", last modified: Fri Jun  2 07:10:47 2023, max compression
+gzip compressed data, was "interactions.py-5.7.0.tar", last modified: Mon Jun 19 07:13:13 2023, max compression
```

## Comparing `interactions.py-5.6.0.tar` & `interactions.py-5.7.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.177320 interactions.py-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-02 07:10:10.000000 interactions.py-5.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-02 07:10:10.000000 interactions.py-5.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-02 07:10:47.177320 interactions.py-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-02 07:10:10.000000 interactions.py-5.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.157320 interactions.py-5.6.0/interactions/
--rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.157320 interactions.py-5.6.0/interactions/api/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.157320 interactions.py-5.6.0/interactions/api/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24007 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.161320 interactions.py-5.6.0/interactions/api/events/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/_template.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/channel_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/guild_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/member_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/message_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/reaction_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/role_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/stage_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/thread_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/user_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/events/processors/voice_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.161320 interactions.py-5.6.0/interactions/api/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/gateway/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/gateway/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.161320 interactions.py-5.6.0/interactions/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.161320 interactions.py-5.6.0/interactions/api/http/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/emojis.py
--rw-r--r--   0 runner    (1001) docker     (123)    35368 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/scheduled_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/http_requests/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/http/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.165320 interactions.py-5.6.0/interactions/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/voice/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/voice/audio_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/voice/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/voice/opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/voice/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/voice/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/api/voice/voice_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.165320 interactions.py-5.6.0/interactions/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/bin/opus-x64.dll
--rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/bin/opus-x86.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.165320 interactions.py-5.6.0/interactions/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/auto_shard_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    92213 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.165320 interactions.py-5.6.0/interactions/client/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/mixins/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/mixins/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/mixins/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/smart_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.169320 interactions.py-5.6.0/interactions/client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/utils/attr_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/utils/attr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/utils/attr_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/utils/deserialise_app_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/utils/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/utils/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/client/utils/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.169320 interactions.py-5.6.0/interactions/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.169320 interactions.py-5.6.0/interactions/ext/debug_extension/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/debug_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/debug_extension/debug_application_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/debug_extension/debug_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/debug_extension/debug_exts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/debug_extension/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/jurigged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.169320 interactions.py-5.6.0/interactions/ext/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/mypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.169320 interactions.py-5.6.0/interactions/ext/prefixed_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/prefixed_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/prefixed_commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/prefixed_commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/prefixed_commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/prefixed_commands/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/prefixed_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/ext/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.169320 interactions.py-5.6.0/interactions/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.173320 interactions.py-5.6.0/interactions/models/discord/
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/app_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   103322 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    96247 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    38399 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/scheduled_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/stage_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    26138 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/user.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/voice_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/discord/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.177320 interactions.py-5.6.0/interactions/models/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/active_voice_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.177320 interactions.py-5.6.0/interactions/models/internal/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/annotations/slash.py
--rw-r--r--   0 runner    (1001) docker     (123)    55760 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/application_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/auto_defer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    36003 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/localisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.177320 interactions.py-5.6.0/interactions/models/internal/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/tasks/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/internal/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.177320 interactions.py-5.6.0/interactions/models/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/misc/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/models/misc/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:10.000000 interactions.py-5.6.0/interactions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.157320 interactions.py-5.6.0/interactions.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-02 07:10:47.000000 interactions.py-5.6.0/interactions.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-02 07:10:47.000000 interactions.py-5.6.0/interactions.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:10:47.000000 interactions.py-5.6.0/interactions.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-02 07:10:47.000000 interactions.py-5.6.0/interactions.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 07:10:47.000000 interactions.py-5.6.0/interactions.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-02 07:10:10.000000 interactions.py-5.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-02 07:10:10.000000 interactions.py-5.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-02 07:10:47.177320 interactions.py-5.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-02 07:10:40.000000 interactions.py-5.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:47.177320 interactions.py-5.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:10:10.000000 interactions.py-5.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-02 07:10:10.000000 interactions.py-5.6.0/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-06-02 07:10:10.000000 interactions.py-5.6.0/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-02 07:10:10.000000 interactions.py-5.6.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-02 07:10:10.000000 interactions.py-5.6.0/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-02 07:10:10.000000 interactions.py-5.6.0/tests/test_cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-02 07:10:10.000000 interactions.py-5.6.0/tests/test_emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-02 07:10:10.000000 interactions.py-5.6.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.655915 interactions.py-5.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-19 07:12:24.000000 interactions.py-5.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-19 07:12:24.000000 interactions.py-5.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-19 07:13:13.655915 interactions.py-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-19 07:12:24.000000 interactions.py-5.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.619915 interactions.py-5.7.0/interactions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.623915 interactions.py-5.7.0/interactions/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.623915 interactions.py-5.7.0/interactions/api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24007 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.627915 interactions.py-5.7.0/interactions/api/events/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/_template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/channel_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/guild_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/member_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/message_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/reaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/role_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/stage_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/thread_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/events/processors/voice_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.627915 interactions.py-5.7.0/interactions/api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/gateway/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/gateway/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.627915 interactions.py-5.7.0/interactions/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.631915 interactions.py-5.7.0/interactions/api/http/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35309 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/http_requests/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/http/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.631915 interactions.py-5.7.0/interactions/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/voice/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/voice/audio_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/voice/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/voice/opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/voice/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/voice/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/api/voice/voice_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.635915 interactions.py-5.7.0/interactions/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/bin/opus-x64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/bin/opus-x86.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.635915 interactions.py-5.7.0/interactions/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/auto_shard_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92213 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.635915 interactions.py-5.7.0/interactions/client/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/mixins/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/mixins/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/mixins/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/smart_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.639915 interactions.py-5.7.0/interactions/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/utils/attr_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/utils/attr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/utils/attr_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/utils/deserialise_app_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/utils/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/client/utils/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.639915 interactions.py-5.7.0/interactions/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.639915 interactions.py-5.7.0/interactions/ext/debug_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/debug_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/debug_extension/debug_application_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/debug_extension/debug_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/debug_extension/debug_exts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/debug_extension/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/jurigged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.643915 interactions.py-5.7.0/interactions/ext/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/mypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.643915 interactions.py-5.7.0/interactions/ext/prefixed_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/prefixed_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/prefixed_commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/prefixed_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/prefixed_commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/prefixed_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/prefixed_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/ext/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.643915 interactions.py-5.7.0/interactions/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.651915 interactions.py-5.7.0/interactions/models/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/app_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103562 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96261 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38399 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/scheduled_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26138 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/voice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/discord/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.655915 interactions.py-5.7.0/interactions/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/active_voice_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.655915 interactions.py-5.7.0/interactions/models/internal/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/annotations/slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55760 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/application_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/auto_defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36003 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/localisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.655915 interactions.py-5.7.0/interactions/models/internal/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/tasks/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/internal/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.655915 interactions.py-5.7.0/interactions/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/misc/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/models/misc/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:24.000000 interactions.py-5.7.0/interactions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.619915 interactions.py-5.7.0/interactions.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-19 07:13:13.000000 interactions.py-5.7.0/interactions.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-19 07:13:13.000000 interactions.py-5.7.0/interactions.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:13:13.000000 interactions.py-5.7.0/interactions.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-19 07:13:13.000000 interactions.py-5.7.0/interactions.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 07:13:13.000000 interactions.py-5.7.0/interactions.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-19 07:12:24.000000 interactions.py-5.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-19 07:12:24.000000 interactions.py-5.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-19 07:13:13.659915 interactions.py-5.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-19 07:13:04.000000 interactions.py-5.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:13.655915 interactions.py-5.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:24.000000 interactions.py-5.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-19 07:12:24.000000 interactions.py-5.7.0/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-06-19 07:12:24.000000 interactions.py-5.7.0/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-19 07:12:24.000000 interactions.py-5.7.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-19 07:12:24.000000 interactions.py-5.7.0/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-19 07:12:24.000000 interactions.py-5.7.0/tests/test_cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-19 07:12:24.000000 interactions.py-5.7.0/tests/test_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-19 07:12:24.000000 interactions.py-5.7.0/tests/utils.py
```

### Comparing `interactions.py-5.6.0/LICENSE` & `interactions.py-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/PKG-INFO` & `interactions.py-5.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions.py
-Version: 5.6.0
+Version: 5.7.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
@@ -68,15 +68,15 @@
 
 In addition to core functionality, `interactions.py` provides a range of optional extensions, allowing you to further customize your bot and add new features with ease.
 
 ## Extensibility
 
 So the base library doesn't do what you want? No problem! With builtin extensions, you are able to extend the functionality of the library. And if none of those pique your interest, there are a myriad of other extension libraries available.
 
-Just type `bot.load("extension")`
+Just type `bot.load_extension("extension")`
 
 <details>
     <summary>Extensions</summary>
 
    ### Prefixed Commands
 
    Prefixed commands, message commands, or legacy commands.
```

### Comparing `interactions.py-5.6.0/README.md` & `interactions.py-5.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 In addition to core functionality, `interactions.py` provides a range of optional extensions, allowing you to further customize your bot and add new features with ease.
 
 ## Extensibility
 
 So the base library doesn't do what you want? No problem! With builtin extensions, you are able to extend the functionality of the library. And if none of those pique your interest, there are a myriad of other extension libraries available.
 
-Just type `bot.load("extension")`
+Just type `bot.load_extension("extension")`
 
 <details>
     <summary>Extensions</summary>
 
    ### Prefixed Commands
 
    Prefixed commands, message commands, or legacy commands.
```

### Comparing `interactions.py-5.6.0/interactions/__init__.py` & `interactions.py-5.7.0/interactions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from .client import (
     __api_version__,
     __py_version__,
     __repo_url__,
     __version__,
     Absent,
     ACTION_ROW_MAX_ITEMS,
@@ -676,14 +677,18 @@
     "Wait",
     "Webhook",
     "WebhookMixin",
     "WebhookTypes",
     "WebSocketOPCode",
 )
 
+if "discord" in sys.modules:
+    get_logger().error(
+        "`import discord` import detected.  Interactions.py is a completely separate library, and is not compatible with d.py models.  Please see https://interactions-py.github.io/interactions.py/Guides/100%20Migration%20From%20D.py/ for how to fix your code."
+    )
 
 ########################################################################################################################
 # Noteworthy Credits
 # LordOfPolls      -- Lead Contributor
 # Eunwoo1104       -- Founder
 # i0bs             -- Ex-Lead Contributor
 # DeltaXWizard     -- Ex-Lead Contributor
```

### Comparing `interactions.py-5.6.0/interactions/api/events/__init__.py` & `interactions.py-5.7.0/interactions/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/base.py` & `interactions.py-5.7.0/interactions/api/events/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import interactions.models as models
 from interactions.client.const import MISSING, AsyncCallable
 from interactions.client.utils.attr_utils import docs
 from interactions.models.discord.snowflake import to_snowflake
 
 if TYPE_CHECKING:
-    from interactions import Client
+    from interactions.client.client import Client
     from interactions.models.discord.snowflake import Snowflake_Type
     from interactions.models.discord.guild import Guild
 
 __all__ = ("BaseEvent", "GuildEvent", "RawGatewayEvent")
 
 _event_reg = re.compile("(?<!^)(?=[A-Z])")
```

### Comparing `interactions.py-5.6.0/interactions/api/events/discord.py` & `interactions.py-5.7.0/interactions/api/events/discord.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/internal.py` & `interactions.py-5.7.0/interactions/api/events/internal.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/__init__.py` & `interactions.py-5.7.0/interactions/api/events/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/_template.py` & `interactions.py-5.7.0/interactions/api/events/processors/_template.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/auto_mod.py` & `interactions.py-5.7.0/interactions/api/events/processors/auto_mod.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/channel_events.py` & `interactions.py-5.7.0/interactions/api/events/processors/channel_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/guild_events.py` & `interactions.py-5.7.0/interactions/api/events/processors/guild_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/integrations.py` & `interactions.py-5.7.0/interactions/api/events/processors/integrations.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/member_events.py` & `interactions.py-5.7.0/interactions/api/events/processors/member_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/message_events.py` & `interactions.py-5.7.0/interactions/api/events/processors/message_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/reaction_events.py` & `interactions.py-5.7.0/interactions/api/events/processors/reaction_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/role_events.py` & `interactions.py-5.7.0/interactions/api/events/processors/role_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/stage_events.py` & `interactions.py-5.7.0/interactions/api/events/processors/stage_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/thread_events.py` & `interactions.py-5.7.0/interactions/api/events/processors/thread_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/user_events.py` & `interactions.py-5.7.0/interactions/api/events/processors/user_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/events/processors/voice_events.py` & `interactions.py-5.7.0/interactions/api/events/processors/voice_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/gateway/gateway.py` & `interactions.py-5.7.0/interactions/api/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/gateway/state.py` & `interactions.py-5.7.0/interactions/api/gateway/state.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/gateway/websocket.py` & `interactions.py-5.7.0/interactions/api/gateway/websocket.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_client.py` & `interactions.py-5.7.0/interactions/api/http/http_client.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/__init__.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/bot.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/bot.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/channels.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/channels.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/emojis.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/emojis.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/guild.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/guild.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from typing import TYPE_CHECKING, List, cast, Mapping, Any
+from typing import TYPE_CHECKING, Any, List, Mapping, cast
 
 import discord_typings
 
 from interactions.client.utils.serializer import dict_filter_none
 from interactions.models.internal.protocols import CanRequest
-from ..route import Route, PAYLOAD_TYPE
+
+from ..route import PAYLOAD_TYPE, Route
 
 __all__ = ("GuildRequests",)
 
 
 if TYPE_CHECKING:
-    from interactions.models.discord.snowflake import Snowflake_Type
     from interactions.models.discord.enums import AuditLogEventType
+    from interactions.models.discord.snowflake import Snowflake_Type
 
 
 class GuildRequests(CanRequest):
     async def get_guilds(
         self,
         limit: int = 200,
         before: "Snowflake_Type | None" = None,
@@ -400,17 +401,14 @@
     ) -> list[discord_typings.RoleData]:
         """
         Modify the position of a role in the guild.
 
         Args:
             guild_id: The ID of the guild
             position_changes: A list of dicts representing the roles to move and their new positions
-
-            ``{"id": role_id, "position": new_position}``
-
             reason: The reason for this action
 
         Returns:
             List of guild roles
 
         """
         payload: PAYLOAD_TYPE = [
```

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/interactions.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/interactions.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/members.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/members.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/messages.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/messages.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/reactions.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/reactions.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/scheduled_events.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/stickers.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/stickers.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/threads.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/threads.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/users.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/users.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/http_requests/webhooks.py` & `interactions.py-5.7.0/interactions/api/http/http_requests/webhooks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/http/route.py` & `interactions.py-5.7.0/interactions/api/http/route.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/voice/audio.py` & `interactions.py-5.7.0/interactions/api/voice/audio.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/voice/audio_writer.py` & `interactions.py-5.7.0/interactions/api/voice/audio_writer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/voice/encryption.py` & `interactions.py-5.7.0/interactions/api/voice/encryption.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/voice/opus.py` & `interactions.py-5.7.0/interactions/api/voice/opus.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/voice/player.py` & `interactions.py-5.7.0/interactions/api/voice/player.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/voice/recorder.py` & `interactions.py-5.7.0/interactions/api/voice/recorder.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/api/voice/voice_gateway.py` & `interactions.py-5.7.0/interactions/api/voice/voice_gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
             self._udp_ka = threading.Thread(target=self._udp_keep_alive, daemon=True)
             self._udp_ka.start()
 
     def _udp_keep_alive(self) -> None:
         keep_alive = b"\xc9\x00\x00\x00\x00\x00\x00\x00\x00"
 
         self.logger.debug("Starting UDP Keep Alive")
-        while not self.socket._closed and not self.ws.closed:
+        while not self.socket._closed and self.ws and not self.ws.closed:
             try:
                 _, writable, _ = select.select([], [self.socket], [], 0)
                 while not writable:
                     _, writable, _ = select.select([], [self.socket], [], 0)
 
                 # discord will never respond to this, but it helps maintain the hole punch
                 self.socket.sendto(keep_alive, (self.voice_ip, self.voice_port))
```

### Comparing `interactions.py-5.6.0/interactions/bin/opus-x64.dll` & `interactions.py-5.7.0/interactions/bin/opus-x64.dll`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/bin/opus-x86.dll` & `interactions.py-5.7.0/interactions/bin/opus-x86.dll`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/__init__.py` & `interactions.py-5.7.0/interactions/client/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/auto_shard_client.py` & `interactions.py-5.7.0/interactions/client/auto_shard_client.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/client.py` & `interactions.py-5.7.0/interactions/client/client.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/const.py` & `interactions.py-5.7.0/interactions/client/const.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/errors.py` & `interactions.py-5.7.0/interactions/client/errors.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/mixins/modal.py` & `interactions.py-5.7.0/interactions/client/mixins/modal.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if typing.TYPE_CHECKING:
     import interactions
 
 __all__ = ("ModalMixin",)
 
 
 class ModalMixin:
-    client: "interactions.Client"
+    client: "interactions.client.client.Client"
     """The client that created this context."""
     responded: bool
     """Whether this context has been responded to."""
     id: Snowflake
     """The interaction ID."""
     token: str
     """The interaction token."""
```

### Comparing `interactions.py-5.6.0/interactions/client/mixins/send.py` & `interactions.py-5.7.0/interactions/client/mixins/send.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import TYPE_CHECKING, Any, Iterable, Optional, Union
 
 import interactions.models as models
+import interactions.models.discord
 from interactions.models.discord.enums import MessageFlags
 
 if TYPE_CHECKING:
     from interactions.client import Client
     from interactions.models.discord.file import UPLOADABLE_TYPE
     from interactions.models.discord.components import BaseComponent
     from interactions.models.discord.embed import Embed
@@ -78,14 +79,26 @@
                 flags = MessageFlags(flags)
             flags = flags | MessageFlags.SUPPRESS_EMBEDS
         if silent:
             if isinstance(flags, int):
                 flags = MessageFlags(flags)
             flags = flags | MessageFlags.SILENT
 
+        if (
+            files
+            and (
+                isinstance(files, Iterable)
+                and any(isinstance(file, interactions.models.discord.message.Attachment) for file in files)
+            )
+            or isinstance(files, interactions.models.discord.message.Attachment)
+        ):
+            raise ValueError(
+                "Attachments are not files. Attachments only contain metadata about the file, not the file itself - to send an attachment, you need to download it first. Check Attachment.url"
+            )
+
         message_payload = models.discord.message.process_message_payload(
             content=content,
             embeds=embeds or embed,
             components=components,
             stickers=stickers,
             allowed_mentions=allowed_mentions,
             reply_to=reply_to,
```

### Comparing `interactions.py-5.6.0/interactions/client/mixins/serialization.py` & `interactions.py-5.7.0/interactions/client/mixins/serialization.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/smart_cache.py` & `interactions.py-5.7.0/interactions/client/smart_cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/utils/__init__.py` & `interactions.py-5.7.0/interactions/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/utils/attr_converters.py` & `interactions.py-5.7.0/interactions/client/utils/attr_converters.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/utils/attr_utils.py` & `interactions.py-5.7.0/interactions/client/utils/attr_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,28 +32,28 @@
 
     Returns:
         The processed metadata dict
     """
     return {"docs": doc_string}
 
 
-def str_validator(self: Any, attribute: attrs.Attribute, value: Any) -> None:
+def str_validator(cls: Any, attribute: attrs.Attribute, value: Any) -> None:
     """
     Validates that the value is a string. Helps convert and ives a warning if it isn't.
 
     Args:
-        self: The instance of the class.
+        cls: The instance of the class.
         attribute: The attr attribute being validated.
         value: The value being validated.
 
     """
     if not isinstance(value, str):
         if value is MISSING:
             return
-        setattr(self, attribute.name, str(value))
+        setattr(cls, attribute.name, str(value))
         get_logger().warning(
             f"Value of {attribute.name} has been automatically converted to a string. Please use strings in future.\n"
             "Note: Discord will always return value as a string"
         )
 
 
 def attrs_validator(
```

### Comparing `interactions.py-5.6.0/interactions/client/utils/attr_utils.pyi` & `interactions.py-5.7.0/interactions/client/utils/attr_utils.pyi`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/utils/cache.py` & `interactions.py-5.7.0/interactions/client/utils/cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/utils/deserialise_app_cmds.py` & `interactions.py-5.7.0/interactions/client/utils/deserialise_app_cmds.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/utils/formatting.py` & `interactions.py-5.7.0/interactions/client/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/utils/input_utils.py` & `interactions.py-5.7.0/interactions/client/utils/input_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         raise TypeError(f"Object of type {type(obj)} is not JSON serializable")
 
     json.dumps = json.Encoder(enc_hook=enc_hook).encode
     json.loads = json.Decoder().decode
 
     json_mode = "msgspec"
 else:
-    import json
+    import json  # type: ignore
 
 get_logger().debug(f"Using {json_mode} for JSON encoding and decoding.")
 
 
 _quotes = {
     '"': '"',
     "‘": "’",  # noqa RUF001
```

### Comparing `interactions.py-5.6.0/interactions/client/utils/misc_utils.py` & `interactions.py-5.7.0/interactions/client/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/utils/serializer.py` & `interactions.py-5.7.0/interactions/client/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/client/utils/text_utils.py` & `interactions.py-5.7.0/interactions/client/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/console.py` & `interactions.py-5.7.0/interactions/ext/console.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/debug_extension/__init__.py` & `interactions.py-5.7.0/interactions/ext/debug_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/debug_extension/debug_application_cmd.py` & `interactions.py-5.7.0/interactions/ext/debug_extension/debug_application_cmd.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/debug_extension/debug_exec.py` & `interactions.py-5.7.0/interactions/ext/debug_extension/debug_exec.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/debug_extension/debug_exts.py` & `interactions.py-5.7.0/interactions/ext/debug_extension/debug_exts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/debug_extension/utils.py` & `interactions.py-5.7.0/interactions/ext/debug_extension/utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/jurigged.py` & `interactions.py-5.7.0/interactions/ext/jurigged.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         AddOperation,
         DeleteOperation,
         UpdateOperation,
         LineDefinition,
     )
 except ModuleNotFoundError:
     get_logger().error(
-        "jurigged not installed, cannot enable jurigged integration.  Install with `pip install interactions[jurigged]`"
+        "jurigged not installed, cannot enable jurigged integration.  Install with `pip install discord-py-interactions[jurigged]`"
     )
     raise
 
 
 __all__ = ("Jurigged", "setup")
```

### Comparing `interactions.py-5.6.0/interactions/ext/mypy/__init__.py` & `interactions.py-5.7.0/interactions/ext/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/paginators.py` & `interactions.py-5.7.0/interactions/ext/paginators.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,44 +348,47 @@
             page.color = self.default_color
 
         return {
             "embeds": [page.to_dict()],
             "components": [c.to_dict() for c in self.create_components()],
         }
 
-    async def send(self, ctx: BaseContext) -> Message:
+    async def send(self, ctx: BaseContext, **kwargs) -> Message:
         """
         Send this paginator.
 
         Args:
             ctx: The context to send this paginator with
+            **kwargs: Additional options to pass to `send`.
 
         Returns:
             The resulting message
 
         """
-        self._message = await ctx.send(**self.to_dict())
+        self._message = await ctx.send(**self.to_dict(), **kwargs)
         self._author_id = ctx.author.id
 
         if self.timeout_interval > 1:
             self._timeout_task = Timeout(self)
             _ = asyncio.create_task(self._timeout_task())
 
         return self._message
 
-    async def reply(self, ctx: "PrefixedContext") -> Message:
+    async def reply(self, ctx: "PrefixedContext", **kwargs) -> Message:
         """
         Reply this paginator to ctx.
 
         Args:
             ctx: The context to reply this paginator with
+            **kwargs: Additional options to pass to `reply`.
+
         Returns:
             The resulting message
         """
-        self._message = await ctx.reply(**self.to_dict())
+        self._message = await ctx.reply(**self.to_dict(), **kwargs)
         self._author_id = ctx.author.id
 
         if self.timeout_interval > 1:
             self._timeout_task = Timeout(self)
             _ = asyncio.create_task(self._timeout_task())
 
         return self._message
```

### Comparing `interactions.py-5.6.0/interactions/ext/prefixed_commands/__init__.py` & `interactions.py-5.7.0/interactions/ext/prefixed_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/prefixed_commands/command.py` & `interactions.py-5.7.0/interactions/ext/prefixed_commands/command.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/prefixed_commands/context.py` & `interactions.py-5.7.0/interactions/ext/prefixed_commands/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, Iterable, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Iterable, Optional, Union
 
 from typing_extensions import Self
 
 from interactions.client.client import Client
 from interactions.client.mixins.send import SendMixin
 from interactions.models.discord.embed import Embed
 from interactions.models.discord.file import UPLOADABLE_TYPE
@@ -76,15 +76,15 @@
         return await self.client.http.create_message(message_payload, self.channel_id, files=files)
 
     async def reply(
         self,
         content: Optional[str] = None,
         embeds: Optional[Union[Iterable[Union[Embed, dict]], Union[Embed, dict]]] = None,
         embed: Optional[Union[Embed, dict]] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> Message:
         """
         Reply to the context's message. Takes all the same attributes as `send`.
 
         Args:
             content: Message text content.
             embeds: Embedded rich content (up to 6000 characters).
```

### Comparing `interactions.py-5.6.0/interactions/ext/prefixed_commands/help.py` & `interactions.py-5.7.0/interactions/ext/prefixed_commands/help.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/prefixed_commands/manager.py` & `interactions.py-5.7.0/interactions/ext/prefixed_commands/manager.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/prefixed_commands/utils.py` & `interactions.py-5.7.0/interactions/ext/prefixed_commands/utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/ext/sentry.py` & `interactions.py-5.7.0/interactions/ext/sentry.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from interactions.client.const import get_logger
 from interactions.models.internal.tasks.task import Task
 
 try:
     import sentry_sdk
 except ModuleNotFoundError:
     get_logger().error(
-        "sentry-sdk not installed, cannot enable sentry integration.  Install with `pip install interactions[sentry]`"
+        "sentry-sdk not installed, cannot enable sentry integration.  Install with `pip install discord-py-interactions[sentry]`"
     )
     raise
 
 from interactions import Client, Extension, listen
 
 __all__ = ("setup", "default_sentry_filter")
```

### Comparing `interactions.py-5.6.0/interactions/models/__init__.py` & `interactions.py-5.7.0/interactions/models/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/__init__.py` & `interactions.py-5.7.0/interactions/models/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/activity.py` & `interactions.py-5.7.0/interactions/models/discord/activity.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/app_perms.py` & `interactions.py-5.7.0/interactions/models/discord/app_perms.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/application.py` & `interactions.py-5.7.0/interactions/models/discord/application.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/asset.py` & `interactions.py-5.7.0/interactions/models/discord/asset.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/auto_mod.py` & `interactions.py-5.7.0/interactions/models/discord/auto_mod.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/base.py` & `interactions.py-5.7.0/interactions/models/discord/base.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/channel.py` & `interactions.py-5.7.0/interactions/models/discord/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -771,14 +771,16 @@
 
 @attrs.define(eq=False, order=False, hash=False, slots=False, kw_only=True)
 class BaseChannel(DiscordObject):
     name: Optional[str] = attrs.field(repr=True, default=None)
     """The name of the channel (1-100 characters)"""
     type: Union[ChannelType, int] = attrs.field(repr=True, converter=ChannelType)
     """The channel topic (0-1024 characters)"""
+    permissions: Optional[Permissions] = attrs.field(repr=False, default=None, converter=optional_c(Permissions))
+    """Calculated permissions for the bot in this channel, only given when using channels as an option with slash commands"""
 
     @classmethod
     def from_dict_factory(cls, data: dict, client: "Client") -> "TYPE_ALL_CHANNEL":
         """
         Creates a channel object of the appropriate type.
 
         Args:
```

### Comparing `interactions.py-5.6.0/interactions/models/discord/color.py` & `interactions.py-5.7.0/interactions/models/discord/color.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/components.py` & `interactions.py-5.7.0/interactions/models/discord/components.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/embed.py` & `interactions.py-5.7.0/interactions/models/discord/embed.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/emoji.py` & `interactions.py-5.7.0/interactions/models/discord/emoji.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,19 @@
 
         """
         if not self._guild_id:
             raise ValueError("Cannot delete emoji, no guild id set.")
 
         await self._client.http.delete_guild_emoji(self._guild_id, self.id, reason=reason)
 
+    @property
+    def url(self) -> str:
+        """CDN url for the emoji."""
+        return f"https://cdn.discordapp.net/emojis/{self.id}.{'gif' if self.animated else 'png'}"
+
 
 def process_emoji_req_format(emoji: Optional[Union[PartialEmoji, dict, str]]) -> Optional[str]:
     """
     Processes the emoji parameter into the str format required by the API.
 
     Args:
         emoji: The emoji to process.
```

### Comparing `interactions.py-5.6.0/interactions/models/discord/enums.py` & `interactions.py-5.7.0/interactions/models/discord/enums.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/file.py` & `interactions.py-5.7.0/interactions/models/discord/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def __attrs_post_init__(self) -> None:
         if self.file_name is None:
             if isinstance(self.file, (IOBase, BinaryIO)):
                 self.file_name = "file"
             else:
                 self.file_name = Path(self.file).name
 
-    def open_file(self) -> BinaryIO:
+    def open_file(self) -> BinaryIO | IOBase:
         """
         Opens the file.
 
         Returns:
             A file-like BinaryIO object.
 
         """
@@ -51,15 +51,15 @@
         if isinstance(self.file, (IOBase, BinaryIO)):
             self.file.close()
 
 
 UPLOADABLE_TYPE = Union[File, IOBase, BinaryIO, Path, str]
 
 
-def open_file(file: UPLOADABLE_TYPE) -> BinaryIO:
+def open_file(file: UPLOADABLE_TYPE) -> BinaryIO | IOBase:
     """
     Opens the file.
 
     Args:
         file: The target file or path to file.
 
     Returns:
```

### Comparing `interactions.py-5.6.0/interactions/models/discord/guild.py` & `interactions.py-5.7.0/interactions/models/discord/guild.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 import asyncio
 import time
 from asyncio import QueueEmpty
 from collections import namedtuple
 from functools import cmp_to_key
-from typing import List, Optional, Union, Set, Dict, Any, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Union
 from warnings import warn
 
 import attrs
 
 import interactions.models as models
-from interactions.client.const import Absent, MISSING, PREMIUM_GUILD_LIMITS
+from interactions.client.const import MISSING, PREMIUM_GUILD_LIMITS, Absent
 from interactions.client.errors import EventLocationNotProvided, NotFound
 from interactions.client.mixins.serialization import DictSerializationMixin
-from interactions.client.utils.attr_converters import optional, list_converter
-from interactions.client.utils.attr_converters import timestamp_converter
+from interactions.client.utils.attr_converters import optional, list_converter, timestamp_converter
 from interactions.client.utils.attr_utils import docs
 from interactions.client.utils.deserialise_app_cmds import deserialize_app_cmds
-from interactions.client.utils.serializer import to_image_data, no_export_meta
-from interactions.models.discord.app_perms import CommandPermissions, ApplicationCommandPermission
+from interactions.client.utils.serializer import no_export_meta, to_image_data
+from interactions.models.discord.app_perms import (
+    ApplicationCommandPermission,
+    CommandPermissions,
+)
 from interactions.models.discord.auto_mod import AutoModRule, BaseAction, BaseTrigger
 from interactions.models.discord.file import UPLOADABLE_TYPE
 from interactions.models.misc.iterator import AsyncIterator
-from .base import DiscordObject, ClientObject
+
+from .base import ClientObject, DiscordObject
 from .enums import (
-    NSFWLevel,
-    Permissions,
-    SystemChannelFlags,
-    VerificationLevel,
+    AuditLogEventType,
+    AutoModEvent,
+    AutoModTriggerType,
+    ChannelType,
     DefaultNotificationLevel,
     ExplicitContentFilterLevel,
-    MFALevel,
-    ChannelType,
+    ForumLayoutType,
     IntegrationExpireBehaviour,
+    MFALevel,
+    NSFWLevel,
+    Permissions,
     ScheduledEventPrivacyLevel,
     ScheduledEventType,
-    AuditLogEventType,
-    AutoModEvent,
-    AutoModTriggerType,
-    ForumLayoutType,
+    SystemChannelFlags,
+    VerificationLevel,
+)
+from .snowflake import (
+    Snowflake_Type,
+    to_optional_snowflake,
+    to_snowflake,
+    to_snowflake_list,
 )
-from .snowflake import to_snowflake, Snowflake_Type, to_optional_snowflake, to_snowflake_list
 
 if TYPE_CHECKING:
-    from interactions.client.client import Client
     from interactions import InteractionCommand
+    from interactions.client.client import Client
 
 __all__ = (
     "GuildBan",
     "BaseGuild",
     "GuildWelcome",
     "GuildPreview",
     "Guild",
@@ -577,15 +585,15 @@
             self._client.cache.place_member_data(self.id, member)
 
         self.chunked.set()
         self.logger.info(
             f"Cached {iterator.total_retrieved} members for {self.id} in {time.perf_counter() - start_time:.2f} seconds"
         )
 
-    async def gateway_chunk(self, wait=True, presences=True) -> None:
+    async def gateway_chunk(self, wait: bool = True, presences: bool = True) -> None:
         """
         Trigger a gateway `get_members` event, populating this object with members.
 
         Args:
             wait: Wait for chunking to be completed before continuing
             presences: Do you need presence data for members?
         """
@@ -594,15 +602,15 @@
         if wait:
             await self.chunked.wait()
 
     async def chunk(self) -> None:
         """Populates all members of this guild using the REST API."""
         await self.http_chunk()
 
-    async def chunk_guild(self, wait=True, presences=True) -> None:
+    async def chunk_guild(self, wait: bool = True, presences: bool = True) -> None:
         """
         Trigger a gateway `get_members` event, populating this object with members.
 
         !!! warning "Depreciation Warning"
             Gateway chunking is deprecated and replaced by http chunking. Use `guild.gateway_chunk` if you need gateway chunking.
 
         Args:
```

### Comparing `interactions.py-5.6.0/interactions/models/discord/invite.py` & `interactions.py-5.7.0/interactions/models/discord/invite.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/message.py` & `interactions.py-5.7.0/interactions/models/discord/message.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/modal.py` & `interactions.py-5.7.0/interactions/models/discord/modal.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/reaction.py` & `interactions.py-5.7.0/interactions/models/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/role.py` & `interactions.py-5.7.0/interactions/models/discord/role.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/scheduled_event.py` & `interactions.py-5.7.0/interactions/models/discord/scheduled_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from interactions.models.discord.file import UPLOADABLE_TYPE
 from interactions.models.discord.snowflake import Snowflake_Type, to_snowflake
 from interactions.models.discord.timestamp import Timestamp
 from .base import DiscordObject
 from .enums import ScheduledEventPrivacyLevel, ScheduledEventType, ScheduledEventStatus
 
 if TYPE_CHECKING:
-    from interactions.client import Client
+    from interactions.client.client import Client
     from interactions.models.discord.channel import GuildStageVoice, GuildVoice
     from interactions.models.discord.guild import Guild
     from interactions.models.discord.user import Member
     from interactions.models.discord.user import User
 
 __all__ = ("ScheduledEvent",)
```

### Comparing `interactions.py-5.6.0/interactions/models/discord/snowflake.py` & `interactions.py-5.7.0/interactions/models/discord/snowflake.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/stage_instance.py` & `interactions.py-5.7.0/interactions/models/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/sticker.py` & `interactions.py-5.7.0/interactions/models/discord/sticker.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,19 @@
 
         """
         if not self._guild_id:
             raise ValueError("You can only delete guild stickers.")
 
         await self._client.http.delete_guild_sticker(self._guild_id, self.id, reason)
 
+    @property
+    def url(self) -> str:
+        """CDN url for the sticker."""
+        return f"https://media.discordapp.net/stickers/{self.id}.webp"
+
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class StickerPack(DiscordObject):
     """Represents a pack of standard stickers."""
 
     stickers: List["Sticker"] = attrs.field(repr=False, factory=list)
     """The stickers in the pack."""
```

### Comparing `interactions.py-5.6.0/interactions/models/discord/team.py` & `interactions.py-5.7.0/interactions/models/discord/team.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/thread.py` & `interactions.py-5.7.0/interactions/models/discord/thread.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/timestamp.py` & `interactions.py-5.7.0/interactions/models/discord/timestamp.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/user.py` & `interactions.py-5.7.0/interactions/models/discord/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     @classmethod
     def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
         if not isinstance(data["avatar"], Asset):
             if data["avatar"]:
                 data["avatar"] = Asset.from_path_hash(client, f"avatars/{data['id']}/{{}}", data["avatar"])
             elif data["discriminator"] == "0":
-                data["avatar"] = Asset(client, f"{Asset.BASE}/embed/avatars/{(int(data['id']) >> 22) % 5}")
+                data["avatar"] = Asset(client, f"{Asset.BASE}/embed/avatars/{(int(data['id']) >> 22) % 6}")
             else:
                 data["avatar"] = Asset(client, f"{Asset.BASE}/embed/avatars/{int(data['discriminator']) % 5}")
         return data
 
     @property
     def tag(self) -> str:
         """Returns the user's Discord tag."""
```

### Comparing `interactions.py-5.6.0/interactions/models/discord/user.pyi` & `interactions.py-5.7.0/interactions/models/discord/user.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,19 @@
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class FakeUserMixin(FakeBaseUserMixin):
     bot: bool
     system: bool
     public_flags: UserFlags
     premium_type: PremiumType
     banner: Optional["Asset"]
+    avatar_decoration: Optional["Asset"]
     accent_color: Optional["Color"]
     activities: list[Activity]
     status: Absent[Status]
+    _fetched: bool
     @classmethod
     def _process_dict(cls, data: Dict[str, Any], client: Client) -> Dict[str, Any]: ...
     @property
     def member_instances(self) -> List["Member"]: ...
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class User(FakeUserMixin, BaseUser): ...
@@ -144,14 +146,15 @@
     def has_role(self, *roles: Union[Snowflake_Type, Role]) -> bool: ...
     async def timeout(
         self,
         communication_disabled_until: Union["Timestamp", datetime, int, float, str, None],
         reason: Absent[str] = ...,
     ) -> dict: ...
     async def move(self, channel_id: Snowflake_Type) -> None: ...
+    async def disconnect(self) -> None: ...
     async def edit(
         self,
         *,
         nickname: Absent[str] = ...,
         roles: Absent[Iterable["Snowflake_Type"]] = ...,
         mute: Absent[bool] = ...,
         deaf: Absent[bool] = ...,
```

### Comparing `interactions.py-5.6.0/interactions/models/discord/voice_state.py` & `interactions.py-5.7.0/interactions/models/discord/voice_state.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/discord/webhooks.py` & `interactions.py-5.7.0/interactions/models/discord/webhooks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/__init__.py` & `interactions.py-5.7.0/interactions/models/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/active_voice_state.py` & `interactions.py-5.7.0/interactions/models/internal/active_voice_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
     async def stop_recording(self) -> dict[int, BytesIO]:
         """
         Stop the recording.
 
         Returns:
             dict[snowflake, BytesIO]: The recorded audio
         """
-        if not self.recorder or not self.recorder.recording:
+        if not self.recorder or not self.recorder.recording or not self.recorder.audio:
             raise RuntimeError("No recorder is running!")
         await self.recorder.stop_recording()
 
         self.recorder.audio.finished.wait()
         return self.recordings
 
     @property
```

### Comparing `interactions.py-5.6.0/interactions/models/internal/annotations/slash.py` & `interactions.py-5.7.0/interactions/models/internal/annotations/slash.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/application_commands.py` & `interactions.py-5.7.0/interactions/models/internal/application_commands.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/auto_defer.py` & `interactions.py-5.7.0/interactions/models/internal/auto_defer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/callback.py` & `interactions.py-5.7.0/interactions/models/internal/callback.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/checks.py` & `interactions.py-5.7.0/interactions/models/internal/checks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/command.py` & `interactions.py-5.7.0/interactions/models/internal/command.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/context.py` & `interactions.py-5.7.0/interactions/models/internal/context.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/converters.py` & `interactions.py-5.7.0/interactions/models/internal/converters.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/cooldowns.py` & `interactions.py-5.7.0/interactions/models/internal/cooldowns.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/extension.py` & `interactions.py-5.7.0/interactions/models/internal/extension.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/listener.py` & `interactions.py-5.7.0/interactions/models/internal/listener.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/localisation.py` & `interactions.py-5.7.0/interactions/models/internal/localisation.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/protocols.py` & `interactions.py-5.7.0/interactions/models/internal/protocols.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/internal/tasks/task.py` & `interactions.py-5.7.0/interactions/models/internal/tasks/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             if isinstance(val, BaseTrigger):
                 self.reschedule(val)
         except Exception as e:
             self.on_error(e)
 
     def _fire(self, fire_time: datetime) -> None:
         """Called when the task is being fired."""
-        self.trigger.last_call_time = fire_time
+        self.trigger.set_last_call_time(fire_time)
         _ = asyncio.create_task(self())
         self.iteration += 1
 
     async def _task_loop(self) -> None:
         """The main task loop to fire the task at the specified time based on triggers configured."""
         while not self._stop.is_set():
             fire_time = self.trigger.next_fire()
```

### Comparing `interactions.py-5.6.0/interactions/models/internal/tasks/triggers.py` & `interactions.py-5.7.0/interactions/models/internal/tasks/triggers.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     def __or__(self, other: "BaseTrigger") -> "OrTrigger":
         return OrTrigger(self, other)
 
     def reschedule(self) -> None:
         """Update the last call time to now"""
         self.last_call_time = datetime.now()
 
+    def set_last_call_time(self, call_time: datetime) -> None:
+        self.last_call_time = call_time
+
     @abstractmethod
     def next_fire(self) -> datetime | None:
         """
         Return the next datetime to fire on.
 
         Returns:
             Datetime if one can be determined. If no datetime can be determined, return None
@@ -110,21 +113,26 @@
 
 
 class OrTrigger(BaseTrigger):
     """Trigger a task when any sub-trigger is fulfilled."""
 
     def __init__(self, *trigger: BaseTrigger) -> None:
         self.triggers: list[BaseTrigger] = list(trigger)
+        self.current_trigger: BaseTrigger = None
+
+    def set_last_call_time(self, call_time: datetime) -> None:
+        self.current_trigger.last_call_time = call_time
 
     def _get_delta(self, d: BaseTrigger) -> timedelta:
         next_fire = d.next_fire()
         return abs(next_fire - self.last_call_time) if next_fire else timedelta.max
 
     def __or__(self, other: "BaseTrigger") -> "OrTrigger":
         self.triggers.append(other)
         return self
 
+    def _set_current_trigger(self) -> BaseTrigger | None:
+        self.current_trigger = self.triggers[0] if len(self.triggers) == 1 else min(self.triggers, key=self._get_delta)
+        return self.current_trigger
+
     def next_fire(self) -> datetime | None:
-        if len(self.triggers) == 1:
-            return self.triggers[0].next_fire()
-        trigger = min(self.triggers, key=self._get_delta)
-        return trigger.next_fire()
+        return self.current_trigger.next_fire() if self._set_current_trigger() else None
```

### Comparing `interactions.py-5.6.0/interactions/models/internal/wait.py` & `interactions.py-5.7.0/interactions/models/internal/wait.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/misc/context_manager.py` & `interactions.py-5.7.0/interactions/models/misc/context_manager.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions/models/misc/iterator.py` & `interactions.py-5.7.0/interactions/models/misc/iterator.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions.py.egg-info/PKG-INFO` & `interactions.py-5.7.0/interactions.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions.py
-Version: 5.6.0
+Version: 5.7.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
@@ -68,15 +68,15 @@
 
 In addition to core functionality, `interactions.py` provides a range of optional extensions, allowing you to further customize your bot and add new features with ease.
 
 ## Extensibility
 
 So the base library doesn't do what you want? No problem! With builtin extensions, you are able to extend the functionality of the library. And if none of those pique your interest, there are a myriad of other extension libraries available.
 
-Just type `bot.load("extension")`
+Just type `bot.load_extension("extension")`
 
 <details>
     <summary>Extensions</summary>
 
    ### Prefixed Commands
 
    Prefixed commands, message commands, or legacy commands.
```

### Comparing `interactions.py-5.6.0/interactions.py.egg-info/SOURCES.txt` & `interactions.py-5.7.0/interactions.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/interactions.py.egg-info/requires.txt` & `interactions.py-5.7.0/interactions.py.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/pyproject.toml` & `interactions.py-5.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interactions.py"
-version = "5.6.0"
+version = "5.7.0"
 description = "Easy, simple, scalable and modular: a Python API wrapper for interactions."
 authors = [
     "LordOfPolls <dev@lordofpolls.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
@@ -80,15 +80,14 @@
 
 [tool.isort]
 profile = "black"
 skip = ["__init__.py"]
 
 [tool.mypy]
 ignore_missing_imports = true
-plugins = "naff.ext.mypy"
 
 [tool.pyright]
 useLibraryCodeForTypes = true
 reportMissingImports = false
 
 [tool.coverage.report]
 exclude_lines = [
```

### Comparing `interactions.py-5.6.0/setup.py` & `interactions.py-5.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/tests/consts.py` & `interactions.py-5.7.0/tests/consts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/tests/test_bot.py` & `interactions.py-5.7.0/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/tests/test_cache.py` & `interactions.py-5.7.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/tests/test_contexts.py` & `interactions.py-5.7.0/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/tests/test_cooldowns.py` & `interactions.py-5.7.0/tests/test_cooldowns.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/tests/test_emoji.py` & `interactions.py-5.7.0/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.6.0/tests/utils.py` & `interactions.py-5.7.0/tests/utils.py`

 * *Files identical despite different names*

