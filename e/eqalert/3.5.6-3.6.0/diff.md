# Comparing `tmp/eqalert-3.5.6.tar.gz` & `tmp/eqalert-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eqalert-3.5.6.tar", last modified: Fri Jun 16 21:17:01 2023, max compression
+gzip compressed data, was "eqalert-3.6.0.tar", last modified: Thu Jun 22 00:07:13 2023, max compression
```

## Comparing `eqalert-3.5.6.tar` & `eqalert-3.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:17:01.853630 eqalert-3.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-06-16 21:17:01.853630 eqalert-3.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-06-16 21:16:35.000000 eqalert-3.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:17:01.845630 eqalert-3.5.6/eqa/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    60680 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/eqalert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:17:01.849630 eqalert-3.5.6/eqa/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   114513 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/action.py
--rw-r--r--   0 runner    (1001) docker     (123)   588543 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    83014 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    85313 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/encounter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31830 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)   488508 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/lib/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:17:01.849630 eqalert-3.5.6/eqa/sound/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/sound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/sound/tick.wav
--rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-16 21:16:35.000000 eqalert-3.5.6/eqa/sound/tock.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:17:01.849630 eqalert-3.5.6/eqalert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-06-16 21:17:01.000000 eqalert-3.5.6/eqalert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 21:17:01.000000 eqalert-3.5.6/eqalert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 21:17:01.000000 eqalert-3.5.6/eqalert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 21:17:01.000000 eqalert-3.5.6/eqalert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-16 21:17:01.000000 eqalert-3.5.6/eqalert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-16 21:17:01.000000 eqalert-3.5.6/eqalert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-16 21:17:01.853630 eqalert-3.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-16 21:16:35.000000 eqalert-3.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:13.886646 eqalert-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-06-22 00:07:13.886646 eqalert-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-06-22 00:06:48.000000 eqalert-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:13.878646 eqalert-3.6.0/eqa/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57500 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/eqalert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:13.882646 eqalert-3.6.0/eqa/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113914 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)   588638 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83035 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86851 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/encounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31830 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)   488508 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/lib/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:13.882646 eqalert-3.6.0/eqa/sound/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/sound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/sound/tick.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-22 00:06:48.000000 eqalert-3.6.0/eqa/sound/tock.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:13.886646 eqalert-3.6.0/eqalert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-06-22 00:07:13.000000 eqalert-3.6.0/eqalert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-22 00:07:13.000000 eqalert-3.6.0/eqalert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:07:13.000000 eqalert-3.6.0/eqalert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 00:07:13.000000 eqalert-3.6.0/eqalert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 00:07:13.000000 eqalert-3.6.0/eqalert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 00:07:13.000000 eqalert-3.6.0/eqalert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 00:07:13.886646 eqalert-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-22 00:06:48.000000 eqalert-3.6.0/setup.py
```

### Comparing `eqalert-3.5.6/PKG-INFO` & `eqalert-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqalert
-Version: 3.5.6
+Version: 3.6.0
 Summary: Configurable and Context Driven Project 1999 Log Parser
 Home-page: https://github.com/mgeitz/eqalert
 Author: M Geitz
 Author-email: git@geitz.xyz
 License: GPL2
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
```

### Comparing `eqalert-3.5.6/README.md` & `eqalert-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/eqa/eqalert.py` & `eqalert-3.6.0/eqa/eqalert.py`

 * *Files 4% similar despite different names*

```diff
@@ -323,14 +323,15 @@
             target=eqa_encounter.process,
             args=(
                 configs,
                 base_path,
                 encounter_q,
                 system_q,
                 display_q,
+                timer_q,
                 exit_flag,
                 cfg_reload,
                 state,
                 version,
             ),
         )
         process_encounter.daemon = True
@@ -371,14 +372,19 @@
                 cfg_reload,
                 change_char,
             ),
         )
         process_timer.daemon = True
         process_timer.start()
 
+        # Sanity check settings dependent on other settings
+        if state.auto_mob_timer and not state.encounter_parse:
+            state.set_encounter_parse(True)
+            eqa_config.set_last_state(state, configs)
+
         # Manage State and Config
         ## Consume system_q
         ## Produce a pleasant experience
         while not exit_flag.is_set():
             # Sleep between empty checks
             queue_size = system_q.qsize()
             if queue_size < 1:
@@ -901,28 +907,26 @@
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Raid mode enabled",
                     )
                 )
-                sound_q.put(eqa_struct.sound("speak", "Raid mode enabled"))
             # Toggle raid state to false
             else:
                 state.set_raid(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Raid mode disabled",
                     )
                 )
-                sound_q.put(eqa_struct.sound("speak", "Raid mode disabled"))
         # Set raid state to true
         elif not state.raid and new_message.rx == True:
             state.set_raid(True)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
@@ -952,36 +956,26 @@
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Raid context will be automatically set by zone",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Raid context will be automatically set by zone"
-                    )
-                )
             # Auto-set raid state to false
             elif not new_message.payload and state.auto_raid:
                 state.set_auto_raid(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Raid context will not be automatically updated",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Raid context will not be automatically updated"
-                    )
-                )
         display_q.put(
             eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system raid: Error on line "
@@ -1036,42 +1030,47 @@
     """Perform system tasks for auto timer behavior"""
 
     try:
         # If timer setting is mob related
         if new_message.rx == "mob":
             # Set auto-mob timer to true
             if not state.auto_mob_timer and new_message.payload:
+                if not state.encounter_parse:
+                    state.set_encounter_parse(True)
+                    eqa_config.set_last_state(state, configs)
+                    display_q.put(
+                        eqa_struct.display(
+                            eqa_settings.eqa_time(),
+                            "event",
+                            "events",
+                            "Encounter Parse Enabled",
+                        )
+                    )
                 state.set_auto_mob_timer(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Automatic mob respawn timers enabled",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound("speak", "Automatic mob respawn timers enabled")
-                )
             # Set auto-mob timer to false
             elif state.auto_mob_timer and not new_message.payload:
                 state.set_auto_mob_timer(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Automatic mob respawn timers disabled",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound("speak", "Automatic mob respawn timers disabled")
-                )
         # If timer setting is spell related
         elif new_message.rx == "spell":
             pass
         display_q.put(
             eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
@@ -1096,168 +1095,117 @@
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers disabled for spells targetting you",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Spell timers disabled for spells targetting you"
-                    )
-                )
             else:
                 state.set_spell_timer_self(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers enabled for spells targetting you",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Spell timers enabled for spells targetting you"
-                    )
-                )
         elif new_message.rx == "other":
             if state.spell_timer_other:
                 state.set_spell_timer_other(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers disabled for spells targetting others",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Spell timers disabled for spells targetting others"
-                    )
-                )
             else:
                 state.set_spell_timer_other(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers enabled for spells targetting others",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Spell timers enabled for spells targetting others"
-                    )
-                )
         elif new_message.rx == "guild":
             if state.spell_timer_guild_only:
                 state.set_spell_timer_guild_only(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will no longer filter for guild members",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Spell timers will no longer filter for guild members"
-                    )
-                )
             else:
                 state.set_spell_timer_guild_only(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will filter for guild members",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Spell timers will filter for guild members"
-                    )
-                )
         elif new_message.rx == "yours":
             if state.spell_timer_yours_only:
                 state.set_spell_timer_yours_only(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will no longer filter only your spells",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Spell timers will no longer filter only your spells"
-                    )
-                )
             else:
                 state.set_spell_timer_yours_only(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will filter for only your spells",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Spell timers will filter for only your spells"
-                    )
-                )
         elif new_message.rx == "guess":
             if state.spell_timer_guess:
                 state.set_spell_timer_guess(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will no longer guess some uncertain spell timers",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak",
-                        "Spell timers will no longer guess some uncertain spell timers",
-                    )
-                )
             else:
                 state.set_spell_timer_guess(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will guess some uncertain spell timers",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Spell timers will guess some uncertain spell timers"
-                    )
-                )
         display_q.put(
             eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system spell timers: Error on line "
@@ -1279,28 +1227,26 @@
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Consider evaluation enabled",
                 )
             )
-            sound_q.put(eqa_struct.sound("speak", "Consider evaluation enabled"))
         # Toggle consider eval state to false
         elif state.consider_eval and not new_message.payload:
             state.set_consider_eval(False)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Consider evaluation disabled",
                 )
             )
-            sound_q.put(eqa_struct.sound("speak", "Consider evaluation disabled"))
         display_q.put(
             eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system consider: Error on line "
@@ -1322,32 +1268,26 @@
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Automatic character detection enabled",
                 )
             )
-            sound_q.put(
-                eqa_struct.sound("speak", "Automatic character detection enabled")
-            )
         # Toggle detect char state to false
         elif state.detect_char and not new_message.payload:
             state.set_detect_char(False)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Automatic character detection disabled",
                 )
             )
-            sound_q.put(
-                eqa_struct.sound("speak", "Automatic character detection disabled")
-            )
         display_q.put(
             eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system consider: Error on line "
@@ -1369,30 +1309,26 @@
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Debug mode enabled",
                 )
             )
-            sound_q.put(
-                eqa_struct.sound("speak", "Displaying and logging all parser output")
-            )
         # Toggle debug state to false
         elif state.debug and new_message.rx == "toggle":
             state.set_debug(False)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Debug mode disabled",
                 )
             )
-            sound_q.put(eqa_struct.sound("speak", "Debug mode disabled"))
         display_q.put(
             eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system debug: Error on line "
@@ -1420,63 +1356,51 @@
                     )
                 )
                 encounter_q.put(
                     eqa_struct.message(
                         eqa_settings.eqa_time(), None, "clear", None, None
                     )
                 )
-                sound_q.put(eqa_struct.sound("speak", "Encounter Parse Enabled"))
             # Toggle encounter parse to false
             else:
                 state.set_encounter_parse(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Encounter Parse Disabled",
                     )
                 )
-                sound_q.put(eqa_struct.sound("speak", "Encounter Parse Disabled"))
         # Set encounter parse save to false
         elif new_message.rx == "save":
             if state.save_parse and not new_message.payload:
                 state.set_encounter_parse_save(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Encounter parse will not save to a file",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Encounter parser will not save to a file"
-                    )
-                )
             # Set encounter parse save to true
             elif not state.save_parse and new_message.payload:
                 state.set_encounter_parse_save(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Encounter parse will automatically save to a file",
                     )
                 )
-                sound_q.put(
-                    eqa_struct.sound(
-                        "speak", "Encounter parser will automatically save to a file"
-                    )
-                )
         # Clear encounter parse stack
         elif new_message.rx == "clear":
             encounter_q.put(
                 eqa_struct.message(eqa_settings.eqa_time(), None, "clear", None, None)
             )
         # End encounter parse and resolve stack
         elif new_message.rx == "end":
```

### Comparing `eqalert-3.5.6/eqa/lib/action.py` & `eqalert-3.6.0/eqa/lib/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,45 +247,46 @@
                                 line_type,
                                 "stop",
                                 None,
                                 check_line,
                             )
                         )
                     elif "mob_slain_" in line_type:
+                        line_clean = re.sub(r"[^\w\s\,\-\'\`]", "", check_line)
+
+                        if line_type == "mob_slain_other":
+                            target, source = line_clean.split(" has been slain by ")
+                        else:
+                            source, target = line_clean.split(" have slain ")
+
+                        if target.lower() in player_list.keys():
+                            target_known = True
+                        else:
+                            target_known = False
+
                         encounter_q.put(
                             eqa_struct.message(
                                 line_time,
                                 line_type,
                                 "stop",
-                                None,
+                                target_known,
                                 check_line,
                             )
                         )
                     elif line_type == "you_new_zone":
                         encounter_q.put(
                             eqa_struct.message(
                                 line_time,
                                 line_type,
                                 "stop",
                                 None,
                                 check_line,
                             )
                         )
 
-                ## Mob Timers
-                if state.auto_mob_timer:
-                    if "experience_" in line_type:
-                        if state.zone is not None:
-                            action_mob_timer(
-                                timer_q,
-                                configs.zones.config["zones"][state.zone]["timer"],
-                                state.auto_mob_timer_delay,
-                                state.zone,
-                            )
-
                 ## Spell Timers
                 if state.spell_timer_self or state.spell_timer_other:
                     ## Other Spell Timers
                     if state.spell_timer_other:
                         if (
                             re.fullmatch(r"^spell\_.+\_other_on$", line_type)
                             is not None
@@ -1660,36 +1661,14 @@
             "find spell cast: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def action_mob_timer(timer_q, timer_seconds, auto_mob_timer_delay, zone):
-    """Set timer for mob spawn using default zone timer value"""
-
-    timer_seconds = timer_seconds - auto_mob_timer_delay
-    if timer_seconds < 0:
-        timer_seconds = 0
-    if auto_mob_timer_delay <= 0:
-        pop_message = "Pop " + str(zone)
-    else:
-        pop_message = (
-            "Pop " + str(zone) + " in " + str(auto_mob_timer_delay) + " seconds."
-        )
-    timer_q.put(
-        eqa_struct.timer(
-            (datetime.datetime.now() + datetime.timedelta(seconds=timer_seconds)),
-            "timer",
-            str(timer_seconds),
-            pop_message,
-        )
-    )
-
-
 def send_alerts(line_type, check_line, configs, sound_q, display_q, mute_list):
     """Send messages to sound and display queues"""
 
     try:
         # Check Sender
         sender = re.findall(r"^([\w\-]+)", check_line)
 
@@ -2108,23 +2087,20 @@
 
 def action_consider_evaluation(sound_q, check_line):
     """Evaluate consider lines"""
 
     try:
         faction, level = check_line.split(" -- ")
         if "threateningly" in faction or "scowls" in faction:
-            if (
-                "gamble" in level
-                or "floor" in level
-                or "tombstone" in level
-                or "formidable" in level
-            ):
-                danger = True
-            else:
+            if "safe opponent" in level:
+                danger = False
+            elif "could probably win this fight" in level:
                 danger = False
+            else:
+                danger = True
         else:
             danger = False
 
         if danger:
             sound_q.put(eqa_struct.sound("speak", "danger"))
         else:
             sound_q.put(eqa_struct.sound("speak", "safe"))
@@ -2813,15 +2789,17 @@
                         and player_list[args[1]]["level"] == 0
                     ):
                         message = "I only know their name"
                     else:
                         message = args[1] + " is "
                         if player_list[args[1]]["level"] > 0:
                             message = (
-                                message + " a level " + player_list[args[1]]["level"]
+                                message
+                                + " a level "
+                                + str(player_list[args[1]]["level"])
                             )
                         if player_list[args[1]]["class"] is not None:
                             message = message + " " + player_list[args[1]]["class"]
                         else:
                             message = message + " character"
                         if player_list[args[1]]["guild"] is not None:
                             message = message + " in " + player_list[args[1]]["guild"]
```

### Comparing `eqalert-3.5.6/eqa/lib/config.py` & `eqalert-3.6.0/eqa/lib/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -14878,14 +14878,19 @@
       "timer": 1800
     },
     "Sleepers Tomb": {
       "indoors": false,
       "raid_mode": true,
       "timer": 28800
     },
+    "Solusek's Eye": {
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1080
+    },
     "South Kaladim": {
       "indoors": true,
       "raid_mode": false,
       "timer": 400
     },
     "Southern Desert of Ro": {
       "indoors": false,
@@ -19739,16 +19744,16 @@
     "spell_line_feeble_mind_you_on": {
       "alert": {},
       "reaction": false,
       "sound": false
     },
     "spell_line_feel_better_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fire_ds_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fire damage shield dropped"
     },
     "spell_line_fire_flame_other_on": {
```

### Comparing `eqalert-3.5.6/eqa/lib/curses.py` & `eqalert-3.6.0/eqa/lib/curses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1973,15 +1973,15 @@
                 ## Show timers
                 while len(timers) > 0:
                     ### Break if there are more timers than room
                     if print_timer_y > int(timer_y * 0.9):
                         break
                     ### Get timer
                     timer = heapq.heappop(timers)
-                    if timer.type != "metronome":
+                    if timer.type == "timer" or timer.type == "spell":
                         ### Duration remaining
                         time_remaining = timer.time - now
                         time_remaining_days = time_remaining.days
                         time_remaining_seconds = time_remaining.seconds
                         timer_hours = (
                             time_remaining_days * 24 + time_remaining_seconds // 3600
                         )
```

### Comparing `eqalert-3.5.6/eqa/lib/encounter.py` & `eqalert-3.6.0/eqa/lib/encounter.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,26 +22,28 @@
 
 import re
 import sys
 import time
 import os
 import json
 from datetime import datetime
+from datetime import timedelta
 from collections import deque
 
 import eqa.lib.settings as eqa_settings
 import eqa.lib.struct as eqa_struct
 
 
 def process(
     configs,
     base_path,
     encounter_q,
     system_q,
     display_q,
+    timer_q,
     exit_flag,
     cfg_reload,
     state,
     version,
 ):
     """
     Process: encounter_q
@@ -60,14 +62,15 @@
 
             # Check queue for message
             if not encounter_q.empty():
                 new_message = encounter_q.get()
                 line_type = new_message.type
                 line_time = new_message.timestamp
                 interaction = new_message.tx
+                interaction_details = new_message.rx
                 line = new_message.payload
 
                 ## Check for encounter_stack clear
                 if interaction == "clear":
                     encounter_stack.clear()
 
                 ## If not an active encounter
@@ -101,18 +104,20 @@
                                     line_type,
                                     line_time,
                                     line,
                                     encounter_stack,
                                     state,
                                     configs,
                                     display_q,
+                                    timer_q,
                                     encounter_zone,
                                     version,
+                                    interaction_details,
                                 )
-                            else:
+                            elif interaction_details == True:
                                 encounter_stack.append(
                                     (
                                         line_time,
                                         source.title(),
                                         target.title(),
                                         "slain",
                                         "other",
@@ -123,32 +128,36 @@
                                 line_type,
                                 line_time,
                                 line,
                                 encounter_stack,
                                 state,
                                 configs,
                                 display_q,
+                                timer_q,
                                 encounter_zone,
                                 version,
+                                interaction_details,
                             )
 
                     if line_type == "you_new_zone":
                         encounter_stack.clear()
 
                     elif interaction == "end":
                         encounter_analysis(
                             line_type,
                             line_time,
                             line,
                             encounter_stack,
                             state,
                             configs,
                             display_q,
+                            timer_q,
                             encounter_zone,
                             version,
+                            interaction_details,
                         )
 
                     elif interaction == "start":
                         #### Set active encounter
                         active_encounter = True
                         if state.zone is not None:
                             encounter_zone = re.sub(r"[^\w\s]", "", state.zone)
@@ -1266,16 +1275,18 @@
     line_type,
     line_time,
     line,
     encounter_stack,
     state,
     configs,
     display_q,
+    timer_q,
     encounter_zone,
     version,
+    target_in_player_list,
 ):
     """Analyze encounter stack before reporting"""
 
     try:
         ## Uncommenting this will print the contents of the encounter stack, update the path
         # import time
 
@@ -1318,15 +1329,19 @@
             line_clean = re.sub(r"[^\w\s\,\-\'\`]", "", line)
             source, target = line_clean.split(" have slain ")
             encounter_target = target.title()
             target_known = True
             end_time = line_time
 
         # If target is not known, let's make a guess
-        if encounter_stack_events > 0 and not target_known:
+        if (
+            encounter_stack_events > 0
+            and not target_known
+            and not target_in_player_list
+        ):
             target_count = {}
             for event in encounter_stack:
                 time, source, target, mode, result = event
 
                 ### Build target count
                 if target not in target_count.keys():
                     target_count[target] = 0
@@ -1417,14 +1432,41 @@
                 encounter_stack,
                 state,
                 configs,
                 display_q,
                 encounter_zone,
                 version,
             )
+
+            # Generate respawn alert
+            if state.auto_mob_timer:
+                default_zone_respawn = configs.zones.config["zones"][state.zone][
+                    "timer"
+                ]
+                timer_seconds = default_zone_respawn - state.auto_mob_timer_delay
+                if state.auto_mob_timer_delay <= 0:
+                    pop_message = "Pop " + encounter_target
+                else:
+                    pop_message = (
+                        encounter_target
+                        + " pop in "
+                        + str(state.auto_mob_timer_delay)
+                        + " seconds"
+                    )
+
+                if timer_seconds > 0:
+                    timer_q.put(
+                        eqa_struct.timer(
+                            datetime.now() + timedelta(seconds=timer_seconds),
+                            "timer",
+                            timer_seconds,
+                            pop_message,
+                        )
+                    )
+
         elif state.debug:
             eqa_settings.log("Encounter Report: Unable to determine encounter target")
 
         # Prune old events
         if encounter_end_time is not None:
             prune_encounter_stack(encounter_end_time, encounter_stack)
```

### Comparing `eqalert-3.5.6/eqa/lib/keys.py` & `eqalert-3.6.0/eqa/lib/keys.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/eqa/lib/log.py` & `eqalert-3.6.0/eqa/lib/log.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/eqa/lib/parser.py` & `eqalert-3.6.0/eqa/lib/parser.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/eqa/lib/settings.py` & `eqalert-3.6.0/eqa/lib/settings.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/eqa/lib/sound.py` & `eqalert-3.6.0/eqa/lib/sound.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/eqa/lib/state.py` & `eqalert-3.6.0/eqa/lib/state.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/eqa/lib/struct.py` & `eqalert-3.6.0/eqa/lib/struct.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/eqa/lib/timer.py` & `eqalert-3.6.0/eqa/lib/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,27 +86,26 @@
                     item_spell = saved_timers["timers"][item]["spell"]
                     item_duration = saved_timers["timers"][item]["duration"]
                     item_landed = datetime.datetime.strptime(
                         saved_timers["timers"][item]["landed"], "%Y-%m-%d %H:%M:%S.%f"
                     )
                     item_payload = saved_timers["timers"][item]["payload"]
                     if item_target == state.char.lower():
-                        spell_seconds_used = (file_saved - item_landed).total_seconds()
-                        spell_seconds_left = (
-                            int(item_duration)
-                            - int(spell_seconds_used)
-                            - state.spell_timer_delay
-                        )
                         item_time = datetime.datetime.now() + datetime.timedelta(
-                            seconds=spell_seconds_left
+                            seconds=int(item_duration)
                         )
+                        item_landed = datetime.datetime.now()
                     else:
                         item_time = datetime.datetime.strptime(
                             saved_timers["timers"][item]["time"], "%Y-%m-%d %H:%M:%S.%f"
                         )
+                        item_landed = datetime.datetime.strptime(
+                            saved_timers["timers"][item]["landed"],
+                            "%Y-%m-%d %H:%M:%S.%f",
+                        )
                     if not item_time <= now:
                         heapq.heappush(
                             timers,
                             eqa_struct.spell_timer(
                                 item_time,
                                 item_type,
                                 item_caster,
@@ -273,23 +272,30 @@
                                 "type": str(timer.type),
                                 "seconds": str(timer.seconds),
                                 "payload": str(timer.payload),
                             }
                         }
                     )
                 elif timer.type == "spell":
+                    if timer.target == state.char.lower():
+                        duration = int(
+                            timer.duration
+                            - (datetime.datetime.now() - timer.landed).total_seconds()
+                        )
+                    else:
+                        duration = timer.duration
                     saved_timers_json["timers"].update(
                         {
                             timer_name: {
                                 "time": str(timer.time),
                                 "type": str(timer.type),
                                 "caster": str(timer.caster),
                                 "target": str(timer.target),
                                 "spell": str(timer.spell),
-                                "duration": str(timer.duration),
+                                "duration": duration,
                                 "landed": str(timer.landed),
                                 "payload": str(timer.payload),
                             }
                         }
                     )
 
             json_data = open(saved_timers_path, "w")
```

### Comparing `eqalert-3.5.6/eqa/lib/watch.py` & `eqalert-3.6.0/eqa/lib/watch.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/eqa/sound/tick.wav` & `eqalert-3.6.0/eqa/sound/tick.wav`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/eqa/sound/tock.wav` & `eqalert-3.6.0/eqa/sound/tock.wav`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/eqalert.egg-info/PKG-INFO` & `eqalert-3.6.0/eqalert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqalert
-Version: 3.5.6
+Version: 3.6.0
 Summary: Configurable and Context Driven Project 1999 Log Parser
 Home-page: https://github.com/mgeitz/eqalert
 Author: M Geitz
 Author-email: git@geitz.xyz
 License: GPL2
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
```

### Comparing `eqalert-3.5.6/eqalert.egg-info/SOURCES.txt` & `eqalert-3.6.0/eqalert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.6/setup.py` & `eqalert-3.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="eqalert",
-    version="3.5.6",
+    version="3.6.0",
     author="M Geitz",
     author_email="git@geitz.xyz",
     install_requires=[
         "playsound>=1.3.0",
         "gtts>=2.3.1",
     ],
     python_requires=">=3.9.2",
```

