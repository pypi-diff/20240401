# Comparing `tmp/secure_email_lacsd-1.0.3.tar.gz` & `tmp/secure_email_lacsd-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure_email_lacsd-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "secure_email_lacsd-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `secure_email_lacsd-1.0.3.tar` & `secure_email_lacsd-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       66 2023-11-16 21:57:59.120998 secure_email_lacsd-1.0.3/.gitattributes
--rw-r--r--   0        0        0       83 2024-03-06 14:52:33.897999 secure_email_lacsd-1.0.3/.gitignore
--rw-r--r--   0        0        0     1097 2024-01-11 21:40:39.534922 secure_email_lacsd-1.0.3/LICENSE
--rw-r--r--   0        0        0   203021 2023-07-27 22:14:13.796814 secure_email_lacsd-1.0.3/demos/attachments/image.png
--rw-r--r--   0        0        0     3855 2023-11-27 19:13:19.439192 secure_email_lacsd-1.0.3/demos/attachments/text_document.txt
--rw-r--r--   0        0        0        0 2023-11-21 19:57:38.749561 secure_email_lacsd-1.0.3/demos/flask_app/__init__.py
--rw-r--r--   0        0        0     2781 2024-01-11 14:52:32.580945 secure_email_lacsd-1.0.3/demos/flask_app/app.py
--rw-r--r--   0        0        0     1005 2023-11-21 16:54:53.207570 secure_email_lacsd-1.0.3/demos/flask_app/templates/index.html
--rw-r--r--   0        0        0      307 2024-01-05 15:02:12.743069 secure_email_lacsd-1.0.3/demos/requirements.txt
--rw-r--r--   0        0        0     3756 2024-03-06 14:52:03.075414 secure_email_lacsd-1.0.3/demos/send_email.py
--rw-r--r--   0        0        0      386 2024-01-11 22:36:20.962755 secure_email_lacsd-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4310 2024-03-06 14:45:18.687891 secure_email_lacsd-1.0.3/readme.md
--rw-r--r--   0        0        0       28 2024-01-17 18:40:04.178661 secure_email_lacsd-1.0.3/requirements.txt
--rw-r--r--   0        0        0        7 2024-01-17 18:40:08.119560 secure_email_lacsd-1.0.3/src/requirements.txt
--rw-r--r--   0        0        0      335 2024-03-06 14:47:38.907756 secure_email_lacsd-1.0.3/src/secure_email/__init__.py
--rw-r--r--   0        0        0     7739 2024-03-06 14:53:01.292950 secure_email_lacsd-1.0.3/src/secure_email/sendmail.py
--rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 secure_email_lacsd-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-11-16 21:57:59.120998 secure_email_lacsd-1.0.4/.gitattributes
+-rw-r--r--   0        0        0       83 2024-03-06 14:52:33.897999 secure_email_lacsd-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1097 2024-01-11 21:40:39.534922 secure_email_lacsd-1.0.4/LICENSE
+-rw-r--r--   0        0        0   203021 2023-07-27 22:14:13.796814 secure_email_lacsd-1.0.4/demos/attachments/image.png
+-rw-r--r--   0        0        0     3855 2023-11-27 19:13:19.439192 secure_email_lacsd-1.0.4/demos/attachments/text_document.txt
+-rw-r--r--   0        0        0        0 2023-11-21 19:57:38.749561 secure_email_lacsd-1.0.4/demos/flask_app/__init__.py
+-rw-r--r--   0        0        0     2781 2024-01-11 14:52:32.580945 secure_email_lacsd-1.0.4/demos/flask_app/app.py
+-rw-r--r--   0        0        0     1005 2023-11-21 16:54:53.207570 secure_email_lacsd-1.0.4/demos/flask_app/templates/index.html
+-rw-r--r--   0        0        0      307 2024-01-05 15:02:12.743069 secure_email_lacsd-1.0.4/demos/requirements.txt
+-rw-r--r--   0        0        0     3943 2024-04-01 15:20:12.610592 secure_email_lacsd-1.0.4/demos/send_email.py
+-rw-r--r--   0        0        0      386 2024-01-11 22:36:20.962755 secure_email_lacsd-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4161 2024-04-01 15:24:04.913912 secure_email_lacsd-1.0.4/readme.md
+-rw-r--r--   0        0        0       28 2024-01-17 18:40:04.178661 secure_email_lacsd-1.0.4/requirements.txt
+-rw-r--r--   0        0        0        7 2024-01-17 18:40:08.119560 secure_email_lacsd-1.0.4/src/requirements.txt
+-rw-r--r--   0        0        0      335 2024-04-01 15:24:22.135844 secure_email_lacsd-1.0.4/src/secure_email/__init__.py
+-rw-r--r--   0        0        0     6923 2024-04-01 15:19:43.604637 secure_email_lacsd-1.0.4/src/secure_email/sendmail.py
+-rw-r--r--   0        0        0     4324 1970-01-01 00:00:00.000000 secure_email_lacsd-1.0.4/PKG-INFO
```

### Comparing `secure_email_lacsd-1.0.3/LICENSE` & `secure_email_lacsd-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `secure_email_lacsd-1.0.3/demos/attachments/image.png` & `secure_email_lacsd-1.0.4/demos/attachments/image.png`

 * *Files identical despite different names*

### Comparing `secure_email_lacsd-1.0.3/demos/attachments/text_document.txt` & `secure_email_lacsd-1.0.4/demos/attachments/text_document.txt`

 * *Files identical despite different names*

### Comparing `secure_email_lacsd-1.0.3/demos/flask_app/app.py` & `secure_email_lacsd-1.0.4/demos/flask_app/app.py`

 * *Files identical despite different names*

### Comparing `secure_email_lacsd-1.0.3/demos/flask_app/templates/index.html` & `secure_email_lacsd-1.0.4/demos/flask_app/templates/index.html`

 * *Files identical despite different names*

### Comparing `secure_email_lacsd-1.0.3/demos/send_email.py` & `secure_email_lacsd-1.0.4/demos/send_email.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,25 +10,42 @@
 sys.path.append(src_path)
 
 from src.secure_email import Emailer
 
 with open("config.json", "r") as f:
     config = json.load(f)
 
-emailer = Emailer(
-    # Either supply a password or set use_keyring to True to use password saved in keyring
-    # See readme for instructions on storing password in keyring
+
+args = [
     config.get("host", ""),
     config.get("port", 0),
     config.get("from", ""),
-    use_keyring=True,
-    unsecure_host=config.get("bu_host", ""),
-    include_ssl_status=True,
+]
+
+kwargs = {
+    "unsecure_host": config.get("bu_host", ""),
+    "include_ssl_status": True,
+}
+
+pw = config.get("password")
+kwargs["user"] = config.get("user")
+if pw:
+    kwargs["password"] = pw
+else:
+    kwargs["use_keyring"] = True
+
+emailer = Emailer(
+    # Either supply a password or set use_keyring to True to use password saved in keyring
+    # See readme for instructions on storing password in keyring
+    *args,
+    **kwargs,
 )
 
+print(emailer.__dict__)
+
 directory = Path(__file__).absolute().parent.joinpath("attachments")
 
 txt = str(directory.joinpath("text_document.txt"))
 img = str(directory.joinpath("image.png"))
 
 menu = [
     "-" * 50,
@@ -54,18 +71,17 @@
     text = ""
     while len(text) < n:
         text = f"{text} {randWord()}".strip()
     return text[:n]
 
 
 def printResult(result):
-    stderr = result.stderr.decode()
-    success = stderr == ""
+    success = result == "success"
     if not success:
-        print(stderr)
+        print(result)
     print(f"Email {'sent successfully' if success else 'failed'}")
 
 
 while True:
     response = input("\n".join(menu))
     if response == "1":
         result = emailer.send(
```

### Comparing `secure_email_lacsd-1.0.3/readme.md` & `secure_email_lacsd-1.0.4/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```
 
 To use keyring to fetch the password in the Emailer class, use the email address associated with the credentials as the name:
 
 ```Python
 keyring.set_password(
   "username@domain.com",
-  "lacsd.org\\username",
+  "username@domain.com",
   "supersecretpassword"
 )
 ```
 
 ## Usage
 
 `from secure_email import Emailer`
@@ -63,15 +63,15 @@
       - subject (str): email subject line
       - body (str): body of email as text or HTML string
       - cc_list (list[str]): recipients to CC (default: [])
       - bcc_list (list[str]): recipients to BCC (default: [])
       - html (bool): whether to send body as HTML (default: False)
       - secure (bool): whether to send over SSL (default: True)
     - Returns:
-      - response (subprocess.CompletedProcess): result returned by cmd.exe after executing email send command
+      - response (str): either "success" or error message
 - Example:
 
   ```Python
   # Supply password directly
   emailer = Emailer(
       "my.emailserver.com",  # host
       0,  # port
@@ -88,20 +88,18 @@
   )
 
   response = emailer.send(
       "recipient@domain.org",  # to
       "Open Immediately!!!",  # subject
       "You may have won $1,000,000. Click the link below to find out",  # body
   )
-  successful = response.stderr != ""
-  exit_code = response.returncode
-  # Successfully sent emails will return an exit code of 0
+  successful = response == "success"
   ```
 
 ### EmailHandler
 
-Extends logging.handlers.SMTPHandler to use the [Emailer](#emailer) class to send emails (see the [logging library documentation](https://docs.python.org/3/library/logging.handlers.html#smtphandler) to learn more about the SMTPHandler). EmailHandler does not add any new methods to SMTPHandler, but it does take an additional argument.
+Extends logging.handlers.SMTPHandler to use the [Emailer](#emailer) class to send emails (see the [logging library documentation](https://docs.python.org/3/library/logging.handlers.html#smtphandler) to learn more about the SMTPHandler). EmailHandler does not add any new methods to SMTPHandler, but it does take additional arguments.
 
 - Additional arguments:
   - send_html (bool): whether to send HTML email instead of plain text (default: False)
   - backup_host (str | None): non-SSL host to send from if SSL host fails
   - include_ssl_status (bool): whether to add line to body of sent emails indicating whether email was sent over SSL default: False)
```

### Comparing `secure_email_lacsd-1.0.3/src/secure_email/sendmail.py` & `secure_email_lacsd-1.0.4/src/secure_email/sendmail.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
-import os
+import mimetypes
 import platform
-import re
-import subprocess
-from datetime import datetime
+import smtplib
+import ssl
+import traceback
+from email.message import EmailMessage
 from logging.handlers import SMTPHandler
+from pathlib import Path
+from typing import Optional, Union
 
 try:
     import keyring
 except ImportError:
     pass
 
 machine = platform.node().lower()
@@ -17,72 +20,42 @@
 
 class Emailer:
     def __init__(
         self,
         secure_host: str,
         port: int,
         email_address: str,
-        password=None,
-        user=None,
+        password: Optional[str] = None,
+        user: Optional[str] = None,
         unsecure_host: str = "",
         use_keyring: bool = False,
         include_ssl_status: bool = False,
     ) -> None:
         self.secure_host: str = secure_host
         self.include_ssl_status: bool = include_ssl_status
         self.bu_host: str = unsecure_host
         self.port: int = port
         self.email_address: str = email_address
         self.user: str = user or email_address
-        self.user = self.email_address
         self.password: str = password or ""
         if use_keyring:
             self.password = keyring.get_password(self.email_address, self.user) or ""
             pass
 
-    def __createMailMessage(
-        self,
-        subject: str,
-        attachments: list[str],
-        cc_list: list[str],
-        bcc_list: list[str],
-        html: bool,
-        secure: bool = True,
-    ) -> str:
-        mail_msg: str = f"Send-MailMessage -From '{self.email_address}' -To $recipients"
-        for cc in cc_list:
-            mail_msg += f" -Cc '{cc}'"
-        for bcc in bcc_list:
-            mail_msg += f" -Bcc '{bcc}'"
-        if len(attachments) > 0:
-            mail_msg += (
-                f""" -Attachments {", ".join([f"'{f}'" for f in attachments])}"""
-            )
-        mail_msg += f" -Subject '{subject}'"
-        mail_msg += " -Body $EmailBody"
-        if html:
-            mail_msg += " -BodyAsHtml"
-        mail_msg += f" -Port {self.port}"
-        if secure:
-            mail_msg += " -UseSSL"
-            mail_msg += f" -Credential $mycreds"
-        mail_msg += f" -smtpserver '{self.secure_host if secure else self.bu_host}'"
-        return mail_msg
-
     def __send(
         self,
-        to,
+        to: Union[str, list[str]],
         subject: str,
         body: str,
         attachments: list[str] = [],
         cc_list: list[str] = [],
         bcc_list: list[str] = [],
         html: bool = False,
         secure: bool = True,
-    ) -> subprocess.CompletedProcess:
+    ) -> str:
         """
         Sends STMP email over TLS using SSL
 
         params
         ------
         to (str|list[str]): email recipient(s)
         subject (str): email subject line
@@ -94,69 +67,74 @@
 
         returns
         -------
         response (subprocess.CompletedProcess): exit code returned by cmd.exe after executing
             email send command
         """
 
-        now: str = re.sub(r"[^0-9]", "", datetime.now().isoformat())
         status_str: str = "SSL" if secure else "non-SSL backup host"
         newline: str = "\n"
         if self.include_ssl_status:
             if html:
                 body += f"<p>Email sent over {status_str}</p>"
             else:
                 body += f"{newline}{newline}*** Email sent over {status_str} ***"
-        tempfile: str = f"email_body_{now}.txt"
-        with open(tempfile, "w") as f:
-            f.write(body)
-
-        to = to if isinstance(to, list) else [to]
+        to = to if isinstance(to, str) else ",".join(to)
 
-        commands = []
-        if secure:
-            commands = [
-                "[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12",
-                "$CurrentSecurityProtocol = [Net.ServicePointManager]::SecurityProtocol",
-            ]
-
-        commands = [
-            *commands,
-            f"""$recipients = {", ".join([f"'{addr}'" for addr in to])}""",
-            f"$username = '{self.user}'",
-            f"$password = '{self.password}'",
-            f"$EmailBody = GET-Content -Raw -Path .\\{tempfile}",
-        ]
+        smtp_server = self.secure_host if secure else self.bu_host
+        msg = EmailMessage()
+        if html:
+            msg.set_content(body, subtype="html")
+        else:
+            msg.set_content(body)
+        msg["Subject"] = subject
+        msg["From"] = self.email_address
+        msg["To"] = to
+        if cc_list is not None:
+            msg["CC"] = ",".join(cc_list)
+        if bcc_list is not None:
+            msg["BCC"] = ",".join(bcc_list)
+        for attachment in attachments:
+            filename = Path(attachment).name
+            mimetype, _ = mimetypes.guess_type(attachment)
+            if mimetype is None:
+                continue
+            maintype, subtype = mimetype.split("/")
+            readmode = "r" if maintype == "text" else "rb"
+            kwargs = {"filename": filename}
+            if maintype != "text":
+                kwargs["maintype"] = maintype
+                kwargs["subtype"] = subtype
+            with open(attachment, readmode) as f:
+                content = f.read()
+                msg.add_attachment(content, **kwargs)  # type: ignore
         if secure:
-            commands = [
-                *commands,
-                "$secpasswd = ConvertTo-SecureString $password -AsPlainText -Force",
-                "$mycreds = New-Object System.Management.Automation.PSCredential ($username, $secpasswd)",
-            ]
-        commands.append(
-            self.__createMailMessage(
-                subject, attachments, cc_list, bcc_list, html, secure=secure
-            ),
-        )
-        command = f'powershell -Command "{" ; ".join(commands)}'
-        command += " ; "
-        response = subprocess.run(f"cmd /c {command}", shell=False, capture_output=True)
-        os.remove(tempfile)
-        return response
+            context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+            context.check_hostname = False
+            context.verify_mode = ssl.CERT_NONE
+        try:
+            with smtplib.SMTP(smtp_server, self.port) as server:
+                if secure:
+                    server.starttls(context=context)
+                    server.login(self.email_address, self.password)
+                server.send_message(msg)
+                return "success"
+        except Exception as e:
+            return f"{e}: {traceback.format_exc}"
 
     def send(
         self,
         to,
         subject: str,
         body: str,
         attachments: list[str] = [],
         cc_list: list[str] = [],
         bcc_list: list[str] = [],
         html: bool = False,
-    ) -> subprocess.CompletedProcess:
+    ) -> str:
         """
         Sends STMP email over TLS using SSL
 
         params
         ------
         to (str|list[str]): email recipient(s)
         subject (str): email subject line
@@ -174,16 +152,15 @@
         kwargs = {
             "attachments": attachments,
             "cc_list": cc_list,
             "bcc_list": bcc_list,
             "html": html,
         }
         response = self.__send(*args, **kwargs)
-        stderr = response.stderr.decode()
-        if stderr != "":
+        if response != "success":
             response = self.__send(*args, **kwargs, secure=False)
         return response
 
 
 class EmailHandler(SMTPHandler):
     def __init__(
         self,
@@ -225,13 +202,11 @@
         try:
             result = self.emailer.send(
                 self.toaddrs,
                 self.getSubject(record),
                 self.format(record),
                 html=self.send_html,
             )
-            stderr = result.stderr.decode()
-            success = stderr == ""
-            if not success:
-                print(stderr)
+            if result != "success":
+                print(result)
         except Exception:
             self.handleError(record)
```

### Comparing `secure_email_lacsd-1.0.3/PKG-INFO` & `secure_email_lacsd-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-email-lacsd
-Version: 1.0.3
+Version: 1.0.4
 Summary: This project allows sending STMP email over TLS using SSL.
 Author-email: John Dyer <johndyer@lacsd.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 
 # Secure Email
 
@@ -34,15 +34,15 @@
 ```
 
 To use keyring to fetch the password in the Emailer class, use the email address associated with the credentials as the name:
 
 ```Python
 keyring.set_password(
   "username@domain.com",
-  "lacsd.org\\username",
+  "username@domain.com",
   "supersecretpassword"
 )
 ```
 
 ## Usage
 
 `from secure_email import Emailer`
@@ -71,15 +71,15 @@
       - subject (str): email subject line
       - body (str): body of email as text or HTML string
       - cc_list (list[str]): recipients to CC (default: [])
       - bcc_list (list[str]): recipients to BCC (default: [])
       - html (bool): whether to send body as HTML (default: False)
       - secure (bool): whether to send over SSL (default: True)
     - Returns:
-      - response (subprocess.CompletedProcess): result returned by cmd.exe after executing email send command
+      - response (str): either "success" or error message
 - Example:
 
   ```Python
   # Supply password directly
   emailer = Emailer(
       "my.emailserver.com",  # host
       0,  # port
@@ -96,21 +96,19 @@
   )
 
   response = emailer.send(
       "recipient@domain.org",  # to
       "Open Immediately!!!",  # subject
       "You may have won $1,000,000. Click the link below to find out",  # body
   )
-  successful = response.stderr != ""
-  exit_code = response.returncode
-  # Successfully sent emails will return an exit code of 0
+  successful = response == "success"
   ```
 
 ### EmailHandler
 
-Extends logging.handlers.SMTPHandler to use the [Emailer](#emailer) class to send emails (see the [logging library documentation](https://docs.python.org/3/library/logging.handlers.html#smtphandler) to learn more about the SMTPHandler). EmailHandler does not add any new methods to SMTPHandler, but it does take an additional argument.
+Extends logging.handlers.SMTPHandler to use the [Emailer](#emailer) class to send emails (see the [logging library documentation](https://docs.python.org/3/library/logging.handlers.html#smtphandler) to learn more about the SMTPHandler). EmailHandler does not add any new methods to SMTPHandler, but it does take additional arguments.
 
 - Additional arguments:
   - send_html (bool): whether to send HTML email instead of plain text (default: False)
   - backup_host (str | None): non-SSL host to send from if SSL host fails
   - include_ssl_status (bool): whether to add line to body of sent emails indicating whether email was sent over SSL default: False)
```

