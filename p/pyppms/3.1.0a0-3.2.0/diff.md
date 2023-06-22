# Comparing `tmp/pyppms-3.1.0a0.tar.gz` & `tmp/pyppms-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppms-3.1.0a0.tar", max compression
+gzip compressed data, was "pyppms-3.2.0.tar", max compression
```

## Comparing `pyppms-3.1.0a0.tar` & `pyppms-3.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-3.1.0a0/README.md
--rw-r--r--   0        0        0     1148 2023-06-20 11:54:30.827850 pyppms-3.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-3.1.0a0/src/pyppms/__init__.py
--rw-r--r--   0        0        0     5657 2023-06-20 11:50:46.845568 pyppms-3.1.0a0/src/pyppms/booking.py
--rw-r--r--   0        0        0     7551 2023-06-20 11:40:07.471530 pyppms-3.1.0a0/src/pyppms/common.py
--rw-r--r--   0        0        0    47070 2023-06-20 11:53:20.255126 pyppms-3.1.0a0/src/pyppms/ppms.py
--rw-r--r--   0        0        0     3944 2023-06-20 11:17:40.009575 pyppms-3.1.0a0/src/pyppms/system.py
--rw-r--r--   0        0        0     2270 2023-06-20 11:17:40.009575 pyppms-3.1.0a0/src/pyppms/user.py
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 pyppms-3.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-3.2.0/README.md
+-rw-r--r--   0        0        0     1146 2023-06-22 14:39:12.742431 pyppms-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-3.2.0/src/pyppms/__init__.py
+-rw-r--r--   0        0        0     5657 2023-06-21 14:22:58.508961 pyppms-3.2.0/src/pyppms/booking.py
+-rw-r--r--   0        0        0     7859 2023-06-22 14:37:37.027448 pyppms-3.2.0/src/pyppms/common.py
+-rw-r--r--   0        0        0      130 2023-06-21 14:22:58.508961 pyppms-3.2.0/src/pyppms/exceptions.py
+-rw-r--r--   0        0        0    47406 2023-06-22 14:34:28.688953 pyppms-3.2.0/src/pyppms/ppms.py
+-rw-r--r--   0        0        0     3944 2023-06-20 11:17:40.009575 pyppms-3.2.0/src/pyppms/system.py
+-rw-r--r--   0        0        0     2270 2023-06-20 11:17:40.009575 pyppms-3.2.0/src/pyppms/user.py
+-rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 pyppms-3.2.0/PKG-INFO
```

### Comparing `pyppms-3.1.0a0/README.md` & `pyppms-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyppms-3.1.0a0/pyproject.toml` & `pyppms-3.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 description = "A Python package to communicate with Stratocore's PUMAPI."
 name = "pyppms"
-version = "3.1.0a0"
+version = "3.2.0"
 
 license = "GPLv3"
 
 authors = [
   "Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>",
   "Laurent Guerard <laurent.guerard@unibas.ch>",
 ]
```

### Comparing `pyppms-3.1.0a0/src/pyppms/booking.py` & `pyppms-3.2.0/src/pyppms/booking.py`

 * *Files identical despite different names*

### Comparing `pyppms-3.1.0a0/src/pyppms/common.py` & `pyppms-3.2.0/src/pyppms/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from datetime import datetime, timedelta
 import csv
 from io import StringIO
 
 from loguru import logger as log
 
+from .exceptions import NoDataError
+
 
 def process_response_values(values):
     """Process (in-place) a list of strings, remove quotes, detect boolean etc.
 
     Check all (str) elements of the given list, remove surrounding double-quotes
     and convert 'true' / 'false' strings into Python booleans.
 
@@ -116,32 +118,36 @@
         data will be logged as a warning, in non-graceful mode they will raise
         an Exception.
 
     Returns
     -------
     list(dict)
         A list with dicts where the latter ones have the same form as produced
-        by the dict_from_single_response() function. Note that when graceful
+        by the dict_from_single_response() function. May be empty in case the
+        PUMAPI response didn't contain any useful data. Note that when graceful
         mode is requested, consistency among the dicts is not guaranteed.
 
     Raises
     ------
+    NoDataError
+        Raised when the response text was too short (less than two lines) and
+        the `graceful` parameter has been set to false.
     ValueError
         Raised when the response text is inconsistent and the `graceful`
         parameter has been set to false, or if parsing fails for any other
         unforeseen reason.
     """
     parsed = []
     try:
         lines = text.splitlines()
         if len(lines) < 2:
-            log.warning("Response expected to have two or more lines: {}", text)
+            log.debug("Response has less than TWO lines: >>>{}<<<", text)
             if not graceful:
-                raise ValueError("Invalid response format!")
-            return parsed
+                raise NoDataError("Invalid response format!")
+            return []
 
         header = lines[0].split(",")
         for i, entry in enumerate(header):
             header[i] = entry.strip()
 
         lines_max = lines_min = len(header)
         for line in lines[1:]:
@@ -170,14 +176,17 @@
         if lines_min != lines_max:
             msg = (
                 "Inconsistent data detected, not all dicts will have the "
                 "same number of elements!"
             )
             log.warning(msg)
 
+    except NoDataError as err:
+        raise err
+
     except Exception as err:
         msg = f"Unable to parse data returned by PUMAPI: {text} - ERROR: {err}"
         log.error(msg)
         raise ValueError(msg) from err
 
     return parsed
```

### Comparing `pyppms-3.1.0a0/src/pyppms/ppms.py` & `pyppms-3.2.0/src/pyppms/ppms.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import requests
 from loguru import logger as log
 
 from .common import dict_from_single_response, parse_multiline_response
 from .user import PpmsUser
 from .system import PpmsSystem
 from .booking import PpmsBooking
+from .exceptions import NoDataError
 
 
 class PpmsConnection:
 
     """Connection object to communicate with a PPMS instance.
 
     Attributes
@@ -35,14 +36,16 @@
     timeout : float
         The timeout value used in the ``requests.post`` calls.
     cache_path : str
         A path to a local directory used for caching responses.
     cache_users_only : bool
         Flag indicating that only PPMS user details will be stored in the
         on-disk cache, nothing else.
+    last_served_from_cache
+        Indicates if the last request was served from the cache or on-line.
     users : dict
         A dict with usernames as keys, mapping to the related
         :py:class:`pyppms.user.PpmsUser` object, serves as a cache during the object's
         lifetime (can be empty if no calls to :py:meth:`get_user()` have been done yet).
     fullname_mapping : dict
         A dict mapping a user's *fullname* ("``<LASTNAME> <FIRSTNAME>``") to the
         corresponding username. Entries are filled in dynamically by the
@@ -103,14 +106,16 @@
         self.status = {
             "auth_state": "NOT_TRIED",
             "auth_response": None,
             "auth_httpstatus": -1,
         }
         self.cache_path = cache
         self.cache_users_only = cache_users_only
+        self.last_served_from_cache = False
+        """Indicates if the last request was served from the cache or on-line."""
 
         # run in cache-only mode (e.g. for testing or off-line usage) if no API
         # key has been specified, skip authentication then:
         if api_key != "":
             self.__authenticate()
         elif cache == "":
             raise RuntimeError(
@@ -121,15 +126,15 @@
         """Try to authenticate to PPMS using the `auth` request.
 
         Raises
         ------
         requests.exceptions.ConnectionError
             Raised in case authentication failed for any reason.
         """
-        log.debug(
+        log.trace(
             "Attempting authentication against {} with key [{}...{}]",
             self.url,
             self.api_key[:2],
             self.api_key[-2:],
         )
         self.status["auth_state"] = "attempting"
         response = self.request("auth")
@@ -162,15 +167,15 @@
             msg = (
                 f"Authenticating against {self.url} with key "
                 f"[{self.api_key[:2]}...{self.api_key[-2:]}] FAILED!"
             )
             log.error(msg)
             raise requests.exceptions.ConnectionError(msg)
 
-        log.info(
+        log.debug(
             "Authentication succeeded, response=[{}], http_status=[{}]",
             response.text,
             response.status_code,
         )
         self.status["auth_state"] = "good"
 
     def request(self, action, parameters={}, skip_cache=False):
@@ -203,26 +208,26 @@
             Raised in case the request is not authorized.
         """
         req_data = {"action": action, "apikey": self.api_key}
         req_data.update(parameters)
         # log.debug("Request parameters: {}", parameters)
 
         response = None
-        read_from_cache = False
         try:
             if skip_cache:  # pragma: no cover
                 raise LookupError("Skipping the cache has been requested")
             response = self.__intercept_read(req_data)
-            read_from_cache = True
+            self.last_served_from_cache = True
         except LookupError as err:
-            log.debug(f"Doing an on-line request: {err}")
+            log.trace(f"Doing an on-line request: {err}")
             response = requests.post(self.url, data=req_data, timeout=self.timeout)
+            self.last_served_from_cache = False
 
         # store the response if it hasn't been read from the cache before:
-        if not read_from_cache:  # pragma: no cover
+        if not self.last_served_from_cache:  # pragma: no cover
             self.__intercept_store(req_data, response)
 
         # NOTE: the HTTP status code returned is always `200` even if
         # authentication failed, so we need to check the actual response *TEXT*
         # to figure out if we have succeeded:
         if "request not authorized" in response.text.lower():
             self.status["auth_state"] = "FAILED"
@@ -385,33 +390,33 @@
         Parameters
         ----------
         keep_users : bool, optional
             If set to `True` the `getuser` sub-directory in the cache location
             will be kept, by default `False`.
         """
         if self.cache_path == "":
-            log.info("No cache path configured, not flushing!")
+            log.debug("No cache path configured, not flushing!")
             return
 
         dirs_to_remove = [self.cache_path]  # by default remove the entire cache dir
         keep_msg = ""
         if keep_users:
             keep_msg = " (keeping user details dirs)"
             dirs_to_remove = []
             cache_dirs = os.listdir(self.cache_path)
             for subdir in cache_dirs:
                 if subdir == "getuser":
                     continue
                 dirs_to_remove.append(os.path.join(self.cache_path, subdir))
 
-        log.info("Flushing the on-disk cache at [{}] {}...", self.cache_path, keep_msg)
+        log.debug("Flushing the on-disk cache at [{}] {}...", self.cache_path, keep_msg)
         for directory in dirs_to_remove:
             try:
                 shutil.rmtree(directory)
-                log.debug("Removed directory [{}].", directory)
+                log.trace("Removed directory [{}].", directory)
             except Exception as ex:  # pylint: disable-msg=broad-except
                 log.warning("Removing the cache at [{}] failed: {}", directory, ex)
 
     def get_admins(self):
         """Get all PPMS administrator users.
 
         Returns
@@ -422,15 +427,15 @@
         response = self.request("getadmins")
 
         admins = response.text.splitlines()
         users = []
         for username in admins:
             user = self.get_user(username)
             users.append(user)
-        log.debug("{} admins in the PPMS database: {}", len(admins), ", ".join(admins))
+        log.trace("{} admins in the PPMS database: {}", len(admins), ", ".join(admins))
         return users
 
     def get_booking(self, system_id, booking_type="get"):
         """Get the current or next booking of a system.
 
         WARNING: if the next booking is requested but it is too far in the future,
         PUMAPI silently ignores it - the response is identical to a system that has no
@@ -473,15 +478,15 @@
             log.error("Requesting booking status for system {} failed!", system_id)
             return None
 
         desc = "any future bookings"
         if booking_type == "get":
             desc = "a currently active booking"
         if not response.text.strip():
-            log.debug("System [{}] doesn't have {}", system_id, desc)
+            log.trace("System [{}] doesn't have {}", system_id, desc)
             return None
 
         return PpmsBooking(response.text, booking_type, system_id)
 
     def get_current_booking(self, system_id):
         """Wrapper for `get_booking()` with 'booking_type' set to 'get'."""
         return self.get_booking(system_id, "get")
@@ -497,24 +502,24 @@
         Returns
         -------
         dict
             A dict with the group details, keys being derived from the header
             line of the PUMAPI response, values from the data line.
         """
         response = self.request("getgroup", {"unitlogin": group_id})
-        log.debug("Group details returned by PPMS (raw): {}", response.text)
+        log.trace("Group details returned by PPMS (raw): {}", response.text)
 
         if not response.text:
             msg = f"Group [{group_id}] is unknown to PPMS"
             log.error(msg)
             raise KeyError(msg)
 
         details = dict_from_single_response(response.text)
 
-        log.debug("Details of group {}: {}", group_id, details)
+        log.trace("Details of group {}: {}", group_id, details)
         return details
 
     def get_group_users(self, unitlogin):
         """Get all members of a group in PPMS.
 
         Parameters
         ----------
@@ -529,15 +534,15 @@
         response = self.request("getgroupusers", {"unitlogin": unitlogin})
 
         members = response.text.splitlines()
         users = []
         for username in members:
             user = self.get_user(username)
             users.append(user)
-        log.debug(
+        log.trace(
             "{} members in PPMS group [{}]: {}",
             len(members),
             unitlogin,
             ", ".join(members),
         )
         return users
 
@@ -548,15 +553,15 @@
         -------
         list(str)
             A list with the group identifiers in PPMS.
         """
         response = self.request("getgroups")
 
         groups = response.text.splitlines()
-        log.debug("{} groups in the PPMS database: {}", len(groups), ", ".join(groups))
+        log.trace("{} groups in the PPMS database: {}", len(groups), ", ".join(groups))
         return groups
 
     def get_next_booking(self, system_id):
         """Wrapper for `get_booking()` with 'booking_type' set to 'next'."""
         return self.get_booking(system_id, "next")
 
     def get_running_sheet(self, core_facility_ref, date, ignore_uncached_users=False):
@@ -588,40 +593,42 @@
             there are no bookings or parsing the response failed.
         """
         bookings = []
         parameters = {
             "plateformid": f"{core_facility_ref}",
             "day": date.strftime("%Y-%m-%d"),
         }
-        log.debug("Requesting runningsheet for {}", parameters["day"])
+        log.trace("Requesting runningsheet for {}", parameters["day"])
         response = self.request("getrunningsheet", parameters)
         try:
             entries = parse_multiline_response(response.text, graceful=False)
+        except NoDataError:
+            # in case no bookings exist the response will be empty!
+            log.trace("Runningsheet for the given day was empty!")
+            return []
         except Exception as err:  # pylint: disable-msg=broad-except
             log.error("Parsing runningsheet details failed: {}", err)
-            # NOTE: in case no future bookings exist the response will be empty!
-            log.error("Possibly the runningsheet is empty as no bookings exist?")
-            log.debug("Runningsheet PUMPAI response was: {}", response.text)
-            return bookings
+            log.trace("Runningsheet PUMPAI response was: >>>{}<<<", response.text)
+            return []
 
         for entry in entries:
             full = entry["User"]
             if full not in self.fullname_mapping:
                 if ignore_uncached_users:
                     log.debug("Ignoring booking for uncached user [{}]", full)
                     continue
 
-                log.info("Booking for an uncached user ({}) found!", full)
+                log.debug("Booking for an uncached user ({}) found!", full)
                 self.update_users()
 
             if full not in self.fullname_mapping:
                 log.error("PPMS doesn't seem to know user [{}], skipping", full)
                 continue
 
-            log.info(
+            log.trace(
                 "Booking for user '{}' ({}) found", self.fullname_mapping[full], full
             )
             system_name = entry["Object"]
             system_ids = self.get_systems_matching("", [system_name])
             if len(system_ids) != 1:
                 # NOTE: more than one result should not happen as PPMS doesn't allow for
                 # multiple systems having the same name - no result might happen though!
@@ -652,15 +659,15 @@
         -------
         dict(pyppms.system.PpmsSystem)
             A dict with `PpmsSystem` objects parsed from the PUMAPI response where
             the system ID (int) is used as the dict's key. If parsing a system
             fails for any reason, the system is skipped entirely.
         """
         if self.systems and not force_refresh:
-            log.debug("Using cached details for {} systems", len(self.systems))
+            log.trace("Using cached details for {} systems", len(self.systems))
         else:
             self.update_systems()
 
         return self.systems
 
     def get_systems_matching(self, localisation, name_contains):
         """Query PPMS for systems with a specific location and name.
@@ -695,15 +702,15 @@
             raise TypeError("`name_contains` must be a list of str, not str!")
 
         loc = localisation
         loc_desc = f"with location matching [{localisation}]"
         if localisation == "":
             loc_desc = "(no location filter given)"
 
-        log.info(
+        log.trace(
             "Querying PPMS for systems {}, name matching any of {}",
             loc_desc,
             name_contains,
         )
         system_ids = []
         systems = self.get_systems()
         for sys_id, system in systems.items():
@@ -712,29 +719,29 @@
                     "System [{}] location ({}) is NOT matching ({}), ignoring",
                     system.name,
                     system.localisation,
                     loc,
                 )
                 continue
 
-            # log.debug('System [{}] is matching location [{}], checking if '
+            # log.trace('System [{}] is matching location [{}], checking if '
             #           'the name is matching any of the valid pattern {}',
             #           system.name, loc, name_contains)
             for valid_name in name_contains:
                 if valid_name in system.name:
                     log.trace("System [{}] matches all criteria", system.name)
                     system_ids.append(sys_id)
                     break
 
             # if sys_id not in system_ids:
-            #     log.debug('System [{}] does NOT match a valid name: {}',
+            #     log.trace('System [{}] does NOT match a valid name: {}',
             #               system.name, name_contains)
 
-        log.info("Found {} bookable systems {}", len(system_ids), loc_desc)
-        log.debug("IDs of matching bookable systems {}: {}", loc_desc, system_ids)
+        log.trace("Found {} bookable systems {}", len(system_ids), loc_desc)
+        log.trace("IDs of matching bookable systems {}: {}", loc_desc, system_ids)
         return system_ids
 
     def get_user(self, login_name, skip_cache=False):
         """Fetch user details from PPMS and create a PpmsUser object from it.
 
         Parameters
         ----------
@@ -819,15 +826,15 @@
         #     u'phone,bcode,affiliation,unitlogin,mustchpwd,mustchbcode,'
         #     u'active\r\n'
         #     u'"pyppms","Python","PumAPI","pyppms@python-facility.example",'
         #     u'"+98 (76) 54 3210","","","pyppms",false,false,'
         #     u'true\r\n'
         # )
         details = dict_from_single_response(response.text)
-        log.debug("Details for user [{}]: {}", login_name, details)
+        log.trace("Details for user [{}]: {}", login_name, details)
         return details
 
     def get_user_experience(self, login=None, system_id=None):
         """Get user experience ("User rights") from PPMS.
 
         Parameters
         ----------
@@ -847,15 +854,15 @@
         if login is not None:
             data["login"] = login
         if system_id is not None:
             data["id"] = system_id
         response = self.request("getuserexp", parameters=data)
 
         parsed = parse_multiline_response(response.text)
-        log.debug(
+        log.trace(
             "Received {} experience entries for filters [user:{}] and [id:{}]",
             len(parsed),
             login,
             system_id,
         )
         return parsed
 
@@ -879,16 +886,16 @@
         if active:
             parameters["active"] = "true"
 
         response = self.request("getusers", parameters)
 
         users = response.text.splitlines()
         active_desc = "active " if active else ""
-        log.info("{} {}users in the PPMS database", len(users), active_desc)
-        log.debug(", ".join(users))
+        log.trace("{} {}users in the PPMS database", len(users), active_desc)
+        log.trace(", ".join(users))
         return users
 
     def get_users(self, force_refresh=False, active_only=True):
         """Get user objects for all (or cached) PPMS users.
 
         Parameters
         ----------
@@ -901,15 +908,15 @@
 
         Returns
         -------
         dict(pyppms.user.PpmsUser)
             A dict of PpmsUser objects with the username (login) as key.
         """
         if self.users and not force_refresh:
-            log.debug("Using cached details for {} users", len(self.users))
+            log.trace("Using cached details for {} users", len(self.users))
         else:
             self.update_users(active_only=active_only)
 
         return self.users
 
     def get_users_emails(self, users=None, active=False):
         """Get a list of user email addresses. WARNING - very slow!
@@ -932,15 +939,15 @@
         if users is None:
             users = self.get_user_ids(active=active)
         for user in users:
             email = self.get_user_dict(user)["email"]
             if not email:
                 log.warning("--- WARNING: no email for user [{}]! ---", user)
                 continue
-            # log.debug("{}: {}", user, email)
+            # log.trace("{}: {}", user, email)
             emails.append(email)
 
         return emails
 
     def get_users_with_access_to_system(self, system_id):
         """Get a list of usernames allowed to book the system with the given ID.
 
@@ -965,22 +972,22 @@
         response = self.request("getsysrights", {"id": system_id})
         # this response has a unique format, so parse it directly here:
         try:
             lines = response.text.splitlines()
             for line in lines:
                 permission, username = line.split(":")
                 if permission.upper() == "D":
-                    log.debug(
+                    log.trace(
                         "User [{}] is deactivated for booking system [{}], skipping",
                         username,
                         system_id,
                     )
                     continue
 
-                log.debug(
+                log.trace(
                     "User [{}] has permission to book system [{}]", username, system_id
                 )
                 users.append(username)
 
         except Exception as err:
             msg = (
                 f"Unable to parse data returned by PUMAPI: {response.text} - "
@@ -1061,16 +1068,16 @@
 
         response = self.request("newuser", req_data)
         if not "OK newuser" in response.text:
             msg = f"Creating new user failed: {response.text}"
             log.error(msg)
             raise RuntimeError(msg)
 
-        log.info("Created user [{}] in PPMS.", login)
-        log.debug("Response was: {}", response.text)
+        log.debug("Created user [{}] in PPMS.", login)
+        log.trace("Response was: {}", response.text)
 
     def remove_user_access_from_system(self, username, system_id):
         """Remove permissions for a user to book a given system in PPMS.
 
         Parameters
         ----------
         username : str
@@ -1149,17 +1156,17 @@
 
         parameters = {"id": system_id, "login": login, "type": permission}
         response = self.request("setright", parameters)
 
         # NOTE: the 'setright' action will accept ANY permission type and return 'done'
         # on the request, so there is no way to check from the response if setting the
         # permission really worked!!
-        # log.debug('Request returned text: {}', response.text)
+        # log.trace('Request returned text: {}', response.text)
         if response.text.lower().strip() == "done":
-            log.debug(
+            log.trace(
                 "User [{}] now has permission level [{}] on system [{}]",
                 login,
                 permission_name(permission),
                 system_id,
             )
             return True
 
@@ -1177,30 +1184,30 @@
     def update_systems(self):
         """Update cached details for all bookable systems from PPMS.
 
         Get the details on all bookable systems from PPMS and store them in the local
         cache. If parsing the PUMAPI response for a system fails for any reason, the
         system is skipped entirely.
         """
-        log.debug("Updating list of bookable systems...")
+        log.trace("Updating list of bookable systems...")
         systems = {}
         parse_fails = 0
         response = self.request("getsystems")
         details = parse_multiline_response(response.text, graceful=False)
         for detail in details:
             try:
                 system = PpmsSystem(detail)
             except ValueError as err:
                 log.error("Error processing `getsystems` response: {}", err)
                 parse_fails += 1
                 continue
 
             systems[system.system_id] = system
 
-        log.debug(
+        log.trace(
             "Updated {} bookable systems from PPMS ({} systems failed parsing)",
             len(systems),
             parse_fails,
         )
 
         self.systems = systems
 
@@ -1221,15 +1228,15 @@
         active_only : bool, optional
             If set to `False` also "inactive" users will be fetched from PPMS,
             by default `True`.
         """
         if not user_ids:
             user_ids = self.get_user_ids(active=active_only)
 
-        log.debug("Updating details on {} users", len(user_ids))
+        log.trace("Updating details on {} users", len(user_ids))
         for user_id in user_ids:
             self.get_user(user_id, skip_cache=True)
 
         log.debug("Collected details on {} users", len(self.users))
 
     def user_exists(self, login):
         """Check if an account with the given login name already exists in PPMS.
```

### Comparing `pyppms-3.1.0a0/src/pyppms/system.py` & `pyppms-3.2.0/src/pyppms/system.py`

 * *Files identical despite different names*

### Comparing `pyppms-3.1.0a0/src/pyppms/user.py` & `pyppms-3.2.0/src/pyppms/user.py`

 * *Files identical despite different names*

### Comparing `pyppms-3.1.0a0/PKG-INFO` & `pyppms-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppms
-Version: 3.1.0a0
+Version: 3.2.0
 Summary: A Python package to communicate with Stratocore's PUMAPI.
 Home-page: https://pypi.org/project/pyppms/
 License: GPLv3
 Keywords: ppms,pumapi,booking-system,reservation-system
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.9,<4.0
```

