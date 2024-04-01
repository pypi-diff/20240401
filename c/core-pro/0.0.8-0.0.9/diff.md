# Comparing `tmp/core_pro-0.0.8.tar.gz` & `tmp/core_pro-0.0.9.tar.gz`

## Comparing `core_pro-0.0.8.tar` & `core_pro-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 core_pro-0.0.8/.idea/.gitignore
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 core_pro-0.0.8/.idea/core_pro.iml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 core_pro-0.0.8/.idea/misc.xml
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 core_pro-0.0.8/.idea/modules.xml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 core_pro-0.0.8/.idea/vcs.xml
--rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 core_pro-0.0.8/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 core_pro-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 core_pro-0.0.8/src/core_pro/GDrive.py
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 core_pro-0.0.8/src/core_pro/GMail.py
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 core_pro-0.0.8/src/core_pro/GSheet.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 core_pro-0.0.8/src/core_pro/GSlide.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 core_pro-0.0.8/src/core_pro/__init__.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 core_pro-0.0.8/src/core_pro/cloud.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 core_pro-0.0.8/src/core_pro/config.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 core_pro-0.0.8/src/core_pro/oop_sql.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 core_pro-0.0.8/src/core_pro/seatalk_bot.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 core_pro-0.0.8/src/core_pro/ultilities.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 core_pro-0.0.8/LICENSE
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 core_pro-0.0.8/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 core_pro-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 core_pro-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 core_pro-0.0.9/sh.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 core_pro-0.0.9/.idea/.gitignore
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 core_pro-0.0.9/.idea/core_pro.iml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 core_pro-0.0.9/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 core_pro-0.0.9/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 core_pro-0.0.9/.idea/vcs.xml
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 core_pro-0.0.9/.idea/workspace.xml
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 core_pro-0.0.9/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 core_pro-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 core_pro-0.0.9/src/core_pro/GDrive.py
+-rw-r--r--   0        0        0    10410 2020-02-02 00:00:00.000000 core_pro-0.0.9/src/core_pro/GMail.py
+-rw-r--r--   0        0        0     8494 2020-02-02 00:00:00.000000 core_pro-0.0.9/src/core_pro/GSheet.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 core_pro-0.0.9/src/core_pro/GSlide.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 core_pro-0.0.9/src/core_pro/__init__.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 core_pro-0.0.9/src/core_pro/cloud.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 core_pro-0.0.9/src/core_pro/config.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 core_pro-0.0.9/src/core_pro/oop_sql.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 core_pro-0.0.9/src/core_pro/seatalk_bot.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 core_pro-0.0.9/src/core_pro/ultilities.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 core_pro-0.0.9/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 core_pro-0.0.9/README.md
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 core_pro-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 core_pro-0.0.9/PKG-INFO
```

### Comparing `core_pro-0.0.8/src/core_pro/GDrive.py` & `core_pro-0.0.9/src/core_pro/GDrive.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import io
-from colorama import Fore
-import mimetypes
-from googleapiclient.http import MediaFileUpload, MediaIoBaseDownload
-from .config import GoogleAuthentication
-
-
-class Drive(GoogleAuthentication):
-    service_type = 'drive'
-
-    def __init__(self, service_type=service_type):
-        super().__init__(service_type)
-        self.status = f'{Fore.LIGHTRED_EX}🦑 Drive:{Fore.RESET}'
-
-    def upload(self, file_dir, name_on_drive: str, folder_id: str):
-        """Upload to drive"""
-        file_metadata = {'name': name_on_drive, 'parents': [folder_id]}
-        content_type, _ = mimetypes.guess_type(file_dir)
-        media = MediaFileUpload(file_dir, mimetype=content_type)
-        fields = 'webContentLink, id, webViewLink'
-        file = self.service.files().create(body=file_metadata, media_body=media, fields=fields).execute()
-        print(f"{self.status} upload file_id: {file.get('id')} folder_id: {folder_id}")
-        return file
-
-    def get_file_info(self, file_id):
-        return self.service.files().get(fileId=file_id).execute()
-
-    def drive_download(self, file_id, download_dir):
-        file_info = self.get_file_info(file_id)
-        request = self.service.files().get_media(fileId=file_id)
-        download_name = file_info['name']
-        save_path = f"{download_dir}/{download_name}"
-        fh = io.FileIO(save_path, 'wb')  # save to somewhere with name...
-        downloader = MediaIoBaseDownload(fh, request)
-        done = False
-        while done is False:
-            status, done = downloader.next_chunk()
-            print(f"Download {int(status.progress() * 100)}%!")
-
-        return save_path
-
-    def create_new_folder(self, name, parent_id=None, return_id=False):
-        """
-        create new folder on Google Drive
-        :param name: Name of folder
-        :param parent_id: id of parent folder , default None
-        :param return_id: return folder id if True
-        :return: return folder id if True
-        """
-
-        file_metadata = {
-            'name': name,
-            'parents': [parent_id],
-            'mimeType': 'application/vnd.google-apps.folder'
-        }
-        if not parent_id:
-            file_metadata.pop('parents')
-        file = self.service.files().create(body=file_metadata,
-                                           fields='id').execute()
-        print(f"Successfully created folder: {name}   Folder ID: {file.get('id')}")
-
-        if return_id:
-            return file.get('id')
-
-    def rename_drive_file(self, spreadsheet_id, new_name):
-        file = {'name': new_name}
-        self.service.files().update(fileId=spreadsheet_id, body=file).execute()
-
-    def download_gsheet(self, file_id, file_location, file_name, file_type):
-        request = self.service.files().export_media(fileId=file_id, mimeType=file_type)
-        fh = io.FileIO(file_location + file_name, mode='wb')
-        downloader = MediaIoBaseDownload(fh, request)
-        done = False
-        while done is False:
-            status, done = downloader.next_chunk()
-            print(f"Download {int(status.progress() * 100)}%.")
-
-    def search_files(self, folder_id):
-        fields = 'nextPageToken, files(id, name, createdTime, modifiedTime)'
-        results = self.service.files().list(q=f"'{folder_id}' in parents and trashed=false", fields=fields).execute()
-        return results.get('files', [])
-
-    def share_publicly(self, file_id):
-        user_permission = {'type': 'anyone', 'role': 'reader'}
-        reponse = self.service.permissions().create(fileId=file_id, body=user_permission, fields='id').execute()
-        print(f"{self.status} share publicly at file: {file_id} {reponse.get('id')}")
-
-    def remove_share_publicly(self, file_id):
-        self.service.permissions().delete(fileId=file_id, permissionId='anyoneWithLink', fields='id').execute()
-        print(f"{self.status} remove share publicly at file: {file_id}")
+import io
+from colorama import Fore
+import mimetypes
+from googleapiclient.http import MediaFileUpload, MediaIoBaseDownload
+from .config import GoogleAuthentication
+
+
+class Drive(GoogleAuthentication):
+    service_type = 'drive'
+
+    def __init__(self, service_type=service_type):
+        super().__init__(service_type)
+        self.status = f'{Fore.LIGHTRED_EX}🦑 Drive:{Fore.RESET}'
+
+    def upload(self, file_dir, name_on_drive: str, folder_id: str):
+        """Upload to drive"""
+        file_metadata = {'name': name_on_drive, 'parents': [folder_id]}
+        content_type, _ = mimetypes.guess_type(file_dir)
+        media = MediaFileUpload(file_dir, mimetype=content_type)
+        fields = 'webContentLink, id, webViewLink'
+        file = self.service.files().create(body=file_metadata, media_body=media, fields=fields).execute()
+        print(f"{self.status} upload file_id: {file.get('id')} folder_id: {folder_id}")
+        return file
+
+    def get_file_info(self, file_id):
+        return self.service.files().get(fileId=file_id).execute()
+
+    def drive_download(self, file_id, download_dir):
+        file_info = self.get_file_info(file_id)
+        request = self.service.files().get_media(fileId=file_id)
+        download_name = file_info['name']
+        save_path = f"{download_dir}/{download_name}"
+        fh = io.FileIO(save_path, 'wb')  # save to somewhere with name...
+        downloader = MediaIoBaseDownload(fh, request)
+        done = False
+        while done is False:
+            status, done = downloader.next_chunk()
+            print(f"Download {int(status.progress() * 100)}%!")
+
+        return save_path
+
+    def create_new_folder(self, name, parent_id=None, return_id=False):
+        """
+        create new folder on Google Drive
+        :param name: Name of folder
+        :param parent_id: id of parent folder , default None
+        :param return_id: return folder id if True
+        :return: return folder id if True
+        """
+
+        file_metadata = {
+            'name': name,
+            'parents': [parent_id],
+            'mimeType': 'application/vnd.google-apps.folder'
+        }
+        if not parent_id:
+            file_metadata.pop('parents')
+        file = self.service.files().create(body=file_metadata,
+                                           fields='id').execute()
+        print(f"Successfully created folder: {name}   Folder ID: {file.get('id')}")
+
+        if return_id:
+            return file.get('id')
+
+    def rename_drive_file(self, spreadsheet_id, new_name):
+        file = {'name': new_name}
+        self.service.files().update(fileId=spreadsheet_id, body=file).execute()
+
+    def download_gsheet(self, file_id, file_location, file_name, file_type):
+        request = self.service.files().export_media(fileId=file_id, mimeType=file_type)
+        fh = io.FileIO(file_location + file_name, mode='wb')
+        downloader = MediaIoBaseDownload(fh, request)
+        done = False
+        while done is False:
+            status, done = downloader.next_chunk()
+            print(f"Download {int(status.progress() * 100)}%.")
+
+    def search_files(self, folder_id):
+        fields = 'nextPageToken, files(id, name, createdTime, modifiedTime)'
+        results = self.service.files().list(q=f"'{folder_id}' in parents and trashed=false", fields=fields).execute()
+        return results.get('files', [])
+
+    def share_publicly(self, file_id):
+        user_permission = {'type': 'anyone', 'role': 'reader'}
+        reponse = self.service.permissions().create(fileId=file_id, body=user_permission, fields='id').execute()
+        print(f"{self.status} share publicly at file: {file_id} {reponse.get('id')}")
+
+    def remove_share_publicly(self, file_id):
+        self.service.permissions().delete(fileId=file_id, permissionId='anyoneWithLink', fields='id').execute()
+        print(f"{self.status} remove share publicly at file: {file_id}")
```

### Comparing `core_pro-0.0.8/src/core_pro/GMail.py` & `core_pro-0.0.9/src/core_pro/GMail.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-import io
-import base64
-import mimetypes
-import os
-from email.mime import audio, base, image, text, multipart
-from email import encoders
-from apiclient import errors
-import pandas as pd
-from .config import GoogleAuthentication
-
-
-class Gmail(GoogleAuthentication):
-    service_type = 'gmail'
-    accepted_domains = ['shopee.com', 'airpay.com', 'seagroup.com', 'ved.com.vn']
-
-    def __init__(self, service_type=service_type):
-        super().__init__(service_type)
-
-    def create_message(self, to, subject, message_text, files=None, cc=None, inline_image=None, sender="me"):
-        """Create a message for an email.
-
-      Args:
-        sender: Email address of the sender, default="me"
-        to: Email address of the receiver.
-        subject: The subject of the email message.
-        message_text: The text of the email message.
-        files: The path to the file to be attached. type = list
-        cc: CC mail
-
-      Returns:
-        An object containing a base64url encoded email object.
-        :param inline_image:
-      """
-        message = multipart.MIMEMultipart('mixed')
-        message['to'] = to
-        message['from'] = sender
-        message['subject'] = subject
-        message['Cc'] = cc
-
-        # inline image:
-
-        if inline_image:
-            for i, image in enumerate(inline_image, 1):
-                message_text += f'<br><img src="cid:image{i}">'
-                msgImage = file_for_attach_mail(image)
-                msgImage.add_header('Content-ID', f'<image{i}>')
-
-                # message.attach(MIMEText(message_text, 'html'))
-                message.attach(msgImage)
-            message.attach(text.MIMEText(message_text, 'html'))
-        else:
-            message.attach(text.MIMEText(message_text, 'html'))
-
-        if files:
-            if not isinstance(files, list):
-                files = [files]
-            print(f"send mail with attach files: {files}")
-            for file in files:
-                msg = file_for_attach_mail(file)
-                if file.split('.')[-1]:
-                    if file.split('.')[-1] == 'xlsx':
-                        msg = base.MIMEBase('application', "vnd.ms-excel")
-                        msg.set_payload(open(file, "rb").read())
-                        encoders.encode_base64(msg)
-                    else:
-                        msg = base.MIMEBase('application', "octet-stream")
-                        msg.set_payload(open(file, "rb").read())
-                        encoders.encode_base64(msg)
-                else:
-                    msg = file_for_attach_mail(file)
-                filename = os.path.basename(file)
-                msg.add_header('Content-Disposition', 'attachment', filename=filename)
-
-                message.attach(msg)
-
-        # return {'raw': base64.urlsafe_b64encode(message.as_bytes()).decode()}
-        return {'raw': base64.urlsafe_b64encode(message.as_string().encode()).decode()}
-
-    def send_message(self, message, user_id="me"):
-        """Send an email message.
-      Args:
-        user_id: User's email address. The special value "me"
-        can be used to indicate the authenticated user.
-        message: Message to be sent.
-
-      Returns:
-        Sent Message.
-      """
-        try:
-            message = (self.service.users().messages().send(userId=user_id, body=message).execute())
-            print(f"Message Id: {message['id']}")
-            return message
-        except errors.HttpError as error:
-            print(f"An error occurred: {error}")
-
-    def send_mail(self, to, subject, message_text, files=None, cc=None, inline_img=None, sender="me", user_id="me"):
-        """
-        send gmail ex: send_mail('edward.nguyen@shopee.com', 'test', 'hello world', ['daily.zip'])
-        :param to: address of the receiver
-        :param subject: email subject
-        :param message_text: content
-        :param files: attach files, default: None
-        :param cc: Cc email, default: None
-        :param sender: sender address, default: "me"
-        :param user_id: default: "me"
-        :return: sent email
-        """
-
-        message = self.create_message(to=to, subject=subject, message_text=message_text, files=files, cc=cc,
-                                      sender=sender, inline_image=inline_img)
-        self.send_message(message, user_id=user_id)
-        print(f"Sent mail: to {to}, subject: {subject} !!")
-
-    def search_single_message(self, query):
-        """
-            Searching email
-            :param query: input your query
-            :return: first item from result list
-            """
-        message_info = self.service.users().messages().list(userId='me', q=query).execute()
-        try:
-            print(f"executed query: {message_info['messages'][0]['id']}")
-            return message_info['messages'][0]['id']
-        except Exception as e:
-            print(e)
-            return None
-
-    def ListMessagesMatchingQuery(self, query, user_id='me'):
-        """List all Messages of the user's mailbox matching the query.
-
-        Args:
-          user_id: User's email address. The special value "me"
-          can be used to indicate the authenticated user.
-          query: String used to filter messages returned.
-          Eg.- 'from:user@some_domain.com' for Messages from a particular sender.
-
-        Returns:
-          List of Messages that match the criteria of the query. Note that the
-          returned list contains Message IDs, you must use get with the
-          appropriate ID to get the details of a Message.
-        """
-        try:
-            response = self.service.users().messages().list(userId=user_id, q=query).execute()
-            messages = []
-            if 'messages' in response:
-                messages.extend(response['messages'])
-
-            while 'nextPageToken' in response:
-                page_token = response['nextPageToken']
-                response = self.service.users().messages().list(userId=user_id, q=query,
-                                                                pageToken=page_token).execute()
-                messages.extend(response['messages'])
-
-            return messages
-        except errors.HttpError as error:
-            print('An error occurred: %s' % error)
-
-    # @classmethod
-    def download_one_from_email(self, messageId, directory, filename):
-        file_names = []
-        file_path = ''
-        try:
-            message = self.service.users().messages().get(userId='me', id=messageId).execute()
-            for part in message['payload']['parts']:
-                if part['filename'] == filename:
-                    # data = part['body'].get('data')
-                    attachmentId = part['body'].get('attachmentId')
-                    attachment_info = self.service.users().messages().attachments().get(userId='me', id=attachmentId,
-                                                                                        messageId=messageId).execute()
-                    data = attachment_info['data']
-                    file_path = directory + part['filename']
-                    file_type = part['filename'].split('.')[1]
-                    if file_type == 'csv':
-                        f = open(file_path, 'wb')
-                        f.write(base64.urlsafe_b64decode(data.encode('UTF-8')))
-                        f.close()
-                    elif file_type == 'xlsx':
-                        decrypted = base64.urlsafe_b64decode(data.encode('UTF-8'))
-                        toread = io.BytesIO()
-                        toread.write(decrypted)
-                        df = pd.read_excel(toread)
-                        df.to_excel(file_path, index=None)
-                    file_names.append(file_path)
-            if len(file_names) > 1:
-                return file_names
-            return file_path
-
-        except errors.HttpError as error:
-            print(f'An error occurred: {str(error)}')
-            return None
-
-    # @classmethod
-    def download_all_from_email(self, messageId, directory):
-        file_names = []
-        try:
-            message = self.service.users().messages().get(userId='me', id=messageId).execute()
-            file_path = ''
-            for part in message['payload']['parts']:
-                if part['filename']:
-                    # data = part['body'].get('data')
-                    attachmentId = part['body'].get('attachmentId')
-                    attachment_info = self.service.users().messages().attachments().get(userId='me', id=attachmentId,
-                                                                                        messageId=messageId).execute()
-                    data = attachment_info['data']
-                    file_path = f"{directory}/{part['filename']}"
-                    file_type = part['filename'].split('.')[1]
-                    if file_type == 'csv':
-                        f = open(file_path, 'wb')
-                        f.write(base64.urlsafe_b64decode(data.encode('UTF-8')))
-                        f.close()
-                    elif file_type == 'xlsx':
-                        decrypted = base64.urlsafe_b64decode(data.encode('UTF-8'))
-                        toread = io.BytesIO()
-                        toread.write(decrypted)
-                        df = pd.read_excel(toread)
-                        df.to_excel(file_path, index=None)
-                    file_names.append(file_path)
-            if len(file_names) > 1:
-                return file_names
-            return file_path
-
-        except errors.HttpError as error:
-            print(f'An error occurred: {error}')
-            return None
-
-
-def file_for_attach_mail(file):
-    content_type, encoding = mimetypes.guess_type(file)
-
-    if content_type is None or encoding is not None:
-        content_type = 'application/octet-stream'
-    main_type, sub_type = content_type.split('/', 1)
-    print(main_type)
-    if main_type == 'text':
-        fp = open(file, 'rb')
-        msg = text.MIMEText(fp.read(), _subtype=sub_type)
-        fp.close()
-    elif main_type == 'image':
-        fp = open(file, 'rb')
-        msg = image.MIMEImage(fp.read(), _subtype=sub_type)
-        fp.close()
-    elif main_type == 'audio':
-        fp = open(file, 'rb')
-        msg = audio.MIMEAudio(fp.read(), _subtype=sub_type)
-        fp.close()
-    else:
-        fp = open(file, 'rb')
-        msg = base.MIMEBase(main_type, sub_type)
-        msg.set_payload(fp.read())
-        fp.close()
-
-    return msg
+import io
+import base64
+import mimetypes
+import os
+from email.mime import audio, base, image, text, multipart
+from email import encoders
+from apiclient import errors
+import pandas as pd
+from .config import GoogleAuthentication
+
+
+class Gmail(GoogleAuthentication):
+    service_type = 'gmail'
+    accepted_domains = ['shopee.com', 'airpay.com', 'seagroup.com', 'ved.com.vn']
+
+    def __init__(self, service_type=service_type):
+        super().__init__(service_type)
+
+    def create_message(self, to, subject, message_text, files=None, cc=None, inline_image=None, sender="me"):
+        """Create a message for an email.
+
+      Args:
+        sender: Email address of the sender, default="me"
+        to: Email address of the receiver.
+        subject: The subject of the email message.
+        message_text: The text of the email message.
+        files: The path to the file to be attached. type = list
+        cc: CC mail
+
+      Returns:
+        An object containing a base64url encoded email object.
+        :param inline_image:
+      """
+        message = multipart.MIMEMultipart('mixed')
+        message['to'] = to
+        message['from'] = sender
+        message['subject'] = subject
+        message['Cc'] = cc
+
+        # inline image:
+
+        if inline_image:
+            for i, image in enumerate(inline_image, 1):
+                message_text += f'<br><img src="cid:image{i}">'
+                msgImage = file_for_attach_mail(image)
+                msgImage.add_header('Content-ID', f'<image{i}>')
+
+                # message.attach(MIMEText(message_text, 'html'))
+                message.attach(msgImage)
+            message.attach(text.MIMEText(message_text, 'html'))
+        else:
+            message.attach(text.MIMEText(message_text, 'html'))
+
+        if files:
+            if not isinstance(files, list):
+                files = [files]
+            print(f"send mail with attach files: {files}")
+            for file in files:
+                msg = file_for_attach_mail(file)
+                if file.split('.')[-1]:
+                    if file.split('.')[-1] == 'xlsx':
+                        msg = base.MIMEBase('application', "vnd.ms-excel")
+                        msg.set_payload(open(file, "rb").read())
+                        encoders.encode_base64(msg)
+                    else:
+                        msg = base.MIMEBase('application', "octet-stream")
+                        msg.set_payload(open(file, "rb").read())
+                        encoders.encode_base64(msg)
+                else:
+                    msg = file_for_attach_mail(file)
+                filename = os.path.basename(file)
+                msg.add_header('Content-Disposition', 'attachment', filename=filename)
+
+                message.attach(msg)
+
+        # return {'raw': base64.urlsafe_b64encode(message.as_bytes()).decode()}
+        return {'raw': base64.urlsafe_b64encode(message.as_string().encode()).decode()}
+
+    def send_message(self, message, user_id="me"):
+        """Send an email message.
+      Args:
+        user_id: User's email address. The special value "me"
+        can be used to indicate the authenticated user.
+        message: Message to be sent.
+
+      Returns:
+        Sent Message.
+      """
+        try:
+            message = (self.service.users().messages().send(userId=user_id, body=message).execute())
+            print(f"Message Id: {message['id']}")
+            return message
+        except errors.HttpError as error:
+            print(f"An error occurred: {error}")
+
+    def send_mail(self, to, subject, message_text, files=None, cc=None, inline_img=None, sender="me", user_id="me"):
+        """
+        send gmail ex: send_mail('edward.nguyen@shopee.com', 'test', 'hello world', ['daily.zip'])
+        :param to: address of the receiver
+        :param subject: email subject
+        :param message_text: content
+        :param files: attach files, default: None
+        :param cc: Cc email, default: None
+        :param sender: sender address, default: "me"
+        :param user_id: default: "me"
+        :return: sent email
+        """
+
+        message = self.create_message(to=to, subject=subject, message_text=message_text, files=files, cc=cc,
+                                      sender=sender, inline_image=inline_img)
+        self.send_message(message, user_id=user_id)
+        print(f"Sent mail: to {to}, subject: {subject} !!")
+
+    def search_single_message(self, query):
+        """
+            Searching email
+            :param query: input your query
+            :return: first item from result list
+            """
+        message_info = self.service.users().messages().list(userId='me', q=query).execute()
+        try:
+            print(f"executed query: {message_info['messages'][0]['id']}")
+            return message_info['messages'][0]['id']
+        except Exception as e:
+            print(e)
+            return None
+
+    def ListMessagesMatchingQuery(self, query, user_id='me'):
+        """List all Messages of the user's mailbox matching the query.
+
+        Args:
+          user_id: User's email address. The special value "me"
+          can be used to indicate the authenticated user.
+          query: String used to filter messages returned.
+          Eg.- 'from:user@some_domain.com' for Messages from a particular sender.
+
+        Returns:
+          List of Messages that match the criteria of the query. Note that the
+          returned list contains Message IDs, you must use get with the
+          appropriate ID to get the details of a Message.
+        """
+        try:
+            response = self.service.users().messages().list(userId=user_id, q=query).execute()
+            messages = []
+            if 'messages' in response:
+                messages.extend(response['messages'])
+
+            while 'nextPageToken' in response:
+                page_token = response['nextPageToken']
+                response = self.service.users().messages().list(userId=user_id, q=query,
+                                                                pageToken=page_token).execute()
+                messages.extend(response['messages'])
+
+            return messages
+        except errors.HttpError as error:
+            print('An error occurred: %s' % error)
+
+    # @classmethod
+    def download_one_from_email(self, messageId, directory, filename):
+        file_names = []
+        file_path = ''
+        try:
+            message = self.service.users().messages().get(userId='me', id=messageId).execute()
+            for part in message['payload']['parts']:
+                if part['filename'] == filename:
+                    # data = part['body'].get('data')
+                    attachmentId = part['body'].get('attachmentId')
+                    attachment_info = self.service.users().messages().attachments().get(userId='me', id=attachmentId,
+                                                                                        messageId=messageId).execute()
+                    data = attachment_info['data']
+                    file_path = directory + part['filename']
+                    file_type = part['filename'].split('.')[1]
+                    if file_type == 'csv':
+                        f = open(file_path, 'wb')
+                        f.write(base64.urlsafe_b64decode(data.encode('UTF-8')))
+                        f.close()
+                    elif file_type == 'xlsx':
+                        decrypted = base64.urlsafe_b64decode(data.encode('UTF-8'))
+                        toread = io.BytesIO()
+                        toread.write(decrypted)
+                        df = pd.read_excel(toread)
+                        df.to_excel(file_path, index=None)
+                    file_names.append(file_path)
+            if len(file_names) > 1:
+                return file_names
+            return file_path
+
+        except errors.HttpError as error:
+            print(f'An error occurred: {str(error)}')
+            return None
+
+    # @classmethod
+    def download_all_from_email(self, messageId, directory):
+        file_names = []
+        try:
+            message = self.service.users().messages().get(userId='me', id=messageId).execute()
+            file_path = ''
+            for part in message['payload']['parts']:
+                if part['filename']:
+                    # data = part['body'].get('data')
+                    attachmentId = part['body'].get('attachmentId')
+                    attachment_info = self.service.users().messages().attachments().get(userId='me', id=attachmentId,
+                                                                                        messageId=messageId).execute()
+                    data = attachment_info['data']
+                    file_path = f"{directory}/{part['filename']}"
+                    file_type = part['filename'].split('.')[1]
+                    if file_type == 'csv':
+                        f = open(file_path, 'wb')
+                        f.write(base64.urlsafe_b64decode(data.encode('UTF-8')))
+                        f.close()
+                    elif file_type == 'xlsx':
+                        decrypted = base64.urlsafe_b64decode(data.encode('UTF-8'))
+                        toread = io.BytesIO()
+                        toread.write(decrypted)
+                        df = pd.read_excel(toread)
+                        df.to_excel(file_path, index=None)
+                    file_names.append(file_path)
+            if len(file_names) > 1:
+                return file_names
+            return file_path
+
+        except errors.HttpError as error:
+            print(f'An error occurred: {error}')
+            return None
+
+
+def file_for_attach_mail(file):
+    content_type, encoding = mimetypes.guess_type(file)
+
+    if content_type is None or encoding is not None:
+        content_type = 'application/octet-stream'
+    main_type, sub_type = content_type.split('/', 1)
+    print(main_type)
+    if main_type == 'text':
+        fp = open(file, 'rb')
+        msg = text.MIMEText(fp.read(), _subtype=sub_type)
+        fp.close()
+    elif main_type == 'image':
+        fp = open(file, 'rb')
+        msg = image.MIMEImage(fp.read(), _subtype=sub_type)
+        fp.close()
+    elif main_type == 'audio':
+        fp = open(file, 'rb')
+        msg = audio.MIMEAudio(fp.read(), _subtype=sub_type)
+        fp.close()
+    else:
+        fp = open(file, 'rb')
+        msg = base.MIMEBase(main_type, sub_type)
+        msg.set_payload(fp.read())
+        fp.close()
+
+    return msg
```

### Comparing `core_pro-0.0.8/src/core_pro/GSheet.py` & `core_pro-0.0.9/src/core_pro/GSheet.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,221 +1,221 @@
-import polars as pl
-import pandas as pd
-from colorama import Fore
-from openpyxl.utils.cell import column_index_from_string, coordinate_from_string
-from .config import GoogleAuthentication
-
-
-class Sheet(GoogleAuthentication):
-    service_type = 'sheets'
-
-    def __init__(self, gsheet_key, service_type=service_type):
-        super().__init__(service_type)
-        self.gsheet_key = gsheet_key
-        self.status = f'{Fore.LIGHTGREEN_EX}🐶 Sheet:{Fore.RESET}'
-
-    def google_sheet_into_df(self,
-                             sheet_name: str,
-                             sheet_range: str,
-                             value_render_option='FORMATTED_VALUE',
-                             polars=True) -> pl.DataFrame:
-        """
-        Read google sheet and return a DataFrame
-        :param value_render_option: default FORMATTED_VALUE, UNFORMATTED_VALUE, FORMULA
-        :param sheet_name: google sheet name
-        :param sheet_range: google sheet range
-        :return: a DataFrame
-        """
-        range_update = f'{sheet_name}!{sheet_range}'
-        result = self.service.spreadsheets().values().get(
-            spreadsheetId=self.gsheet_key,
-            range=range_update,
-            valueRenderOption=value_render_option,
-        ).execute()
-        print(f"{self.status} Loaded at {range_update}, Polar: {polars}")
-        if polars:
-            return pl.DataFrame(result['values'][1:], schema=result['values'][0])
-        else:
-            return pd.DataFrame(result['values'][1:], columns=result['values'][0])
-
-    def create_new_gsheet(self, title: str) -> str:
-        """
-        Create new google sheet
-        :param title: title for new google sheet
-        :return: None
-        """
-        spreadsheet = {
-            'properties': {
-                'title': title
-            }
-        }
-        spreadsheet = self.service.spreadsheets().create(body=spreadsheet, fields='spreadsheetId').execute()
-        print(f"Spreadsheet ID: {spreadsheet.get('spreadsheetId')}")
-        spreadsheet_id = spreadsheet.get('spreadsheetId')
-        return spreadsheet_id
-
-    def clear_gsheet(self, sheet_name: str, sheet_range: str):
-        """
-        Clear google sheet
-        :param sheet_name: sheet name
-        :param sheet_range: ex: "A:C"
-        :return: None
-        """
-        name = f'{sheet_name}!{sheet_range}'
-        self.service.spreadsheets().values().clear(spreadsheetId=self.gsheet_key, range=name, body={}).execute()
-
-    def update_value_single_axis(self, sheet_range: str, sheet_name: str, values, value_input='RAW'):
-        """
-        update google sheet value
-        :param sheet_range: range update ex: 'A1'
-        :param sheet_name: sheet name
-        :param values: [[2, 3, 4], [2, 3, 4]]
-        :param value_input: default = 'RAW', or 'USER_ENTERED' or INPUT_VALUE_OPTION_UNSPECIFIED
-        :return: result
-        """
-        range_update = f"{sheet_name}!{sheet_range}"
-        body = {
-            'values': values,
-            'majorDimension': 'ROWS'
-        }
-        self.service.spreadsheets().values().update(
-            spreadsheetId=self.gsheet_key,
-            range=range_update,
-            valueInputOption=value_input,
-            body=body
-        ).execute()
-        print(f"{self.status} Updated at {range_update}")
-
-    def make_a_copy_sheet(self, sheet_id: str, dup_sheet_name: str):
-        """
-        Para:
-        - spreadsheet_id: template_sheet
-        - sheet_id: template_worksheet
-        - dup_sheet_name: sheet to copy
-        """
-
-        duplicated_spreadsheet_body = {'destination_spreadsheet_id': dup_sheet_name}
-        request = self.service.spreadsheets().sheets().copyTo(spreadsheetId=self.gsheet_key,
-                                                              sheetId=sheet_id,
-                                                              body=duplicated_spreadsheet_body)
-        response = request.execute()
-        return response
-
-    def rename_worksheet(self, sheet_id: str, new_title: str):
-        requests = {
-            "updateSheetProperties": {
-                "properties": {
-                    "sheetId": sheet_id,
-                    "title": new_title,
-                },
-                "fields": "title",
-            }
-        }
-        body = {
-            'requests': requests
-        }
-        self.service.spreadsheets().batchUpdate(spreadsheetId=self.gsheet_key, body=body).execute()
-
-    def delete_worksheet(self, sheet_id: str):
-        requests = {
-            "deleteSheet": {
-                "sheetId": sheet_id
-            }
-        }
-        body = {
-            'requests': requests
-        }
-        self.service.spreadsheets().batchUpdate(spreadsheetId=self.gsheet_key, body=body).execute()
-
-    def get_worksheet_properties(self, sheet_name: str):
-        spreadsheet = self.service.spreadsheets().get(spreadsheetId=self.gsheet_key).execute()
-        lst_worksheet = list(filter(lambda x: x.get('properties').get('title') == sheet_name, spreadsheet['sheets']))
-        if lst_worksheet:
-            return lst_worksheet[0].get('properties')
-
-    def format_title(self, ws_id: str, start: str):
-        color_orange = hex_to_rgb('#ff6d01', 'sheets')
-        pos_row = column_index_from_string(coordinate_from_string(start)[0]) - 1
-        pos_col = coordinate_from_string(start)[1]
-        my_range = {
-            'sheetId': ws_id,
-            'startRowIndex': pos_row,
-            'endRowIndex': pos_row + 1,
-            'startColumnIndex': pos_col - 1,
-            'endColumnIndex': pos_col,
-        }
-        request = [
-            {
-                'repeatCell': {
-                    'range': my_range,
-                    'cell': {
-                        'userEnteredFormat': {
-                            'textFormat': {'foregroundColor': color_orange,
-                                           'bold': True,
-                                           'fontSize': 12,
-                                           'fontFamily': 'Roboto'}
-                        }
-                    },
-                    'fields': 'userEnteredFormat(backgroundColor,textFormat)'
-                }
-            },
-        ]
-        body = {"requests": request}
-        self.service.spreadsheets().batchUpdate(spreadsheetId=self.gsheet_key, body=body).execute()
-        print(f'{self.status} Format title at {start}')
-
-    def format_header(self, ws_id: str, start: str, num_col: int):
-        color_grey = hex_to_rgb('#b7b7b7', 'sheets')
-        pos_row = coordinate_from_string(start)[1] - 1
-        pos_col = column_index_from_string(coordinate_from_string(start)[0]) - 1
-
-        my_range = {
-            'sheetId': ws_id,
-            'startRowIndex': pos_row,
-            'endRowIndex': pos_row + 1,
-            'startColumnIndex': pos_col,
-            'endColumnIndex': pos_col + num_col,
-        }
-        request = [
-            {
-                'repeatCell': {
-                    'range': my_range,
-                    'cell': {
-                        'userEnteredFormat': {
-                            'backgroundColor': color_grey,
-                            'horizontalAlignment': 'CENTER',
-                            'textFormat': {'bold': True,
-                                           'fontFamily': 'Roboto'}
-                        }
-                    },
-                    'fields': 'userEnteredFormat(backgroundColor,textFormat,horizontalAlignment)'
-                }
-            },
-        ]
-        body = {"requests": request}
-        self.service.spreadsheets().batchUpdate(spreadsheetId=self.gsheet_key, body=body).execute()
-        print(f'{self.status} Format header at {start}')
-
-    def frozen_view(self, ws_id: str, rows: int = 2):
-        request = [
-            {
-                'updateSheetProperties': {
-                    'properties': {
-                        'sheetId': ws_id,
-                        'gridProperties': {'frozenRowCount': rows}
-                    },
-                    'fields': 'gridProperties.frozenRowCount'
-                }
-            }
-        ]
-        body = {"requests": request}
-        self.service.spreadsheets().batchUpdate(spreadsheetId=self.gsheet_key, body=body).execute()
-        print(f'{self.status} Frozen views')
-
-
-def hex_to_rgb(hex_code, mode='sheets'):
-    hex_code = hex_code.lstrip('#')
-    rgb = tuple(int(hex_code[i:i+2], 16) for i in (0, 2, 4))
-    if mode == 'sheets':
-        return {i: v / 255 for i, v in zip(['red', 'green', 'blue'], rgb)}
-    else:
-        return rgb
+import polars as pl
+import pandas as pd
+from colorama import Fore
+from openpyxl.utils.cell import column_index_from_string, coordinate_from_string
+from .config import GoogleAuthentication
+
+
+class Sheet(GoogleAuthentication):
+    service_type = 'sheets'
+
+    def __init__(self, gsheet_key, service_type=service_type):
+        super().__init__(service_type)
+        self.gsheet_key = gsheet_key
+        self.status = f'{Fore.LIGHTGREEN_EX}🐶 Sheet:{Fore.RESET}'
+
+    def google_sheet_into_df(self,
+                             sheet_name: str,
+                             sheet_range: str,
+                             value_render_option='FORMATTED_VALUE',
+                             polars=True) -> pl.DataFrame:
+        """
+        Read google sheet and return a DataFrame
+        :param value_render_option: default FORMATTED_VALUE, UNFORMATTED_VALUE, FORMULA
+        :param sheet_name: google sheet name
+        :param sheet_range: google sheet range
+        :return: a DataFrame
+        """
+        range_update = f'{sheet_name}!{sheet_range}'
+        result = self.service.spreadsheets().values().get(
+            spreadsheetId=self.gsheet_key,
+            range=range_update,
+            valueRenderOption=value_render_option,
+        ).execute()
+        print(f"{self.status} Loaded at {range_update}, Polar: {polars}")
+        if polars:
+            return pl.DataFrame(result['values'][1:], schema=result['values'][0])
+        else:
+            return pd.DataFrame(result['values'][1:], columns=result['values'][0])
+
+    def create_new_gsheet(self, title: str) -> str:
+        """
+        Create new google sheet
+        :param title: title for new google sheet
+        :return: None
+        """
+        spreadsheet = {
+            'properties': {
+                'title': title
+            }
+        }
+        spreadsheet = self.service.spreadsheets().create(body=spreadsheet, fields='spreadsheetId').execute()
+        print(f"Spreadsheet ID: {spreadsheet.get('spreadsheetId')}")
+        spreadsheet_id = spreadsheet.get('spreadsheetId')
+        return spreadsheet_id
+
+    def clear_gsheet(self, sheet_name: str, sheet_range: str):
+        """
+        Clear google sheet
+        :param sheet_name: sheet name
+        :param sheet_range: ex: "A:C"
+        :return: None
+        """
+        name = f'{sheet_name}!{sheet_range}'
+        self.service.spreadsheets().values().clear(spreadsheetId=self.gsheet_key, range=name, body={}).execute()
+
+    def update_value_single_axis(self, sheet_range: str, sheet_name: str, values, value_input='RAW'):
+        """
+        update google sheet value
+        :param sheet_range: range update ex: 'A1'
+        :param sheet_name: sheet name
+        :param values: [[2, 3, 4], [2, 3, 4]]
+        :param value_input: default = 'RAW', or 'USER_ENTERED' or INPUT_VALUE_OPTION_UNSPECIFIED
+        :return: result
+        """
+        range_update = f"{sheet_name}!{sheet_range}"
+        body = {
+            'values': values,
+            'majorDimension': 'ROWS'
+        }
+        self.service.spreadsheets().values().update(
+            spreadsheetId=self.gsheet_key,
+            range=range_update,
+            valueInputOption=value_input,
+            body=body
+        ).execute()
+        print(f"{self.status} Updated at {range_update}")
+
+    def make_a_copy_sheet(self, sheet_id: str, dup_sheet_name: str):
+        """
+        Para:
+        - spreadsheet_id: template_sheet
+        - sheet_id: template_worksheet
+        - dup_sheet_name: sheet to copy
+        """
+
+        duplicated_spreadsheet_body = {'destination_spreadsheet_id': dup_sheet_name}
+        request = self.service.spreadsheets().sheets().copyTo(spreadsheetId=self.gsheet_key,
+                                                              sheetId=sheet_id,
+                                                              body=duplicated_spreadsheet_body)
+        response = request.execute()
+        return response
+
+    def rename_worksheet(self, sheet_id: str, new_title: str):
+        requests = {
+            "updateSheetProperties": {
+                "properties": {
+                    "sheetId": sheet_id,
+                    "title": new_title,
+                },
+                "fields": "title",
+            }
+        }
+        body = {
+            'requests': requests
+        }
+        self.service.spreadsheets().batchUpdate(spreadsheetId=self.gsheet_key, body=body).execute()
+
+    def delete_worksheet(self, sheet_id: str):
+        requests = {
+            "deleteSheet": {
+                "sheetId": sheet_id
+            }
+        }
+        body = {
+            'requests': requests
+        }
+        self.service.spreadsheets().batchUpdate(spreadsheetId=self.gsheet_key, body=body).execute()
+
+    def get_worksheet_properties(self, sheet_name: str):
+        spreadsheet = self.service.spreadsheets().get(spreadsheetId=self.gsheet_key).execute()
+        lst_worksheet = list(filter(lambda x: x.get('properties').get('title') == sheet_name, spreadsheet['sheets']))
+        if lst_worksheet:
+            return lst_worksheet[0].get('properties')
+
+    def format_title(self, ws_id: str, start: str):
+        color_orange = hex_to_rgb('#ff6d01', 'sheets')
+        pos_row = column_index_from_string(coordinate_from_string(start)[0]) - 1
+        pos_col = coordinate_from_string(start)[1]
+        my_range = {
+            'sheetId': ws_id,
+            'startRowIndex': pos_row,
+            'endRowIndex': pos_row + 1,
+            'startColumnIndex': pos_col - 1,
+            'endColumnIndex': pos_col,
+        }
+        request = [
+            {
+                'repeatCell': {
+                    'range': my_range,
+                    'cell': {
+                        'userEnteredFormat': {
+                            'textFormat': {'foregroundColor': color_orange,
+                                           'bold': True,
+                                           'fontSize': 12,
+                                           'fontFamily': 'Roboto'}
+                        }
+                    },
+                    'fields': 'userEnteredFormat(backgroundColor,textFormat)'
+                }
+            },
+        ]
+        body = {"requests": request}
+        self.service.spreadsheets().batchUpdate(spreadsheetId=self.gsheet_key, body=body).execute()
+        print(f'{self.status} Format title at {start}')
+
+    def format_header(self, ws_id: str, start: str, num_col: int):
+        color_grey = hex_to_rgb('#b7b7b7', 'sheets')
+        pos_row = coordinate_from_string(start)[1] - 1
+        pos_col = column_index_from_string(coordinate_from_string(start)[0]) - 1
+
+        my_range = {
+            'sheetId': ws_id,
+            'startRowIndex': pos_row,
+            'endRowIndex': pos_row + 1,
+            'startColumnIndex': pos_col,
+            'endColumnIndex': pos_col + num_col,
+        }
+        request = [
+            {
+                'repeatCell': {
+                    'range': my_range,
+                    'cell': {
+                        'userEnteredFormat': {
+                            'backgroundColor': color_grey,
+                            'horizontalAlignment': 'CENTER',
+                            'textFormat': {'bold': True,
+                                           'fontFamily': 'Roboto'}
+                        }
+                    },
+                    'fields': 'userEnteredFormat(backgroundColor,textFormat,horizontalAlignment)'
+                }
+            },
+        ]
+        body = {"requests": request}
+        self.service.spreadsheets().batchUpdate(spreadsheetId=self.gsheet_key, body=body).execute()
+        print(f'{self.status} Format header at {start}')
+
+    def frozen_view(self, ws_id: str, rows: int = 2):
+        request = [
+            {
+                'updateSheetProperties': {
+                    'properties': {
+                        'sheetId': ws_id,
+                        'gridProperties': {'frozenRowCount': rows}
+                    },
+                    'fields': 'gridProperties.frozenRowCount'
+                }
+            }
+        ]
+        body = {"requests": request}
+        self.service.spreadsheets().batchUpdate(spreadsheetId=self.gsheet_key, body=body).execute()
+        print(f'{self.status} Frozen views')
+
+
+def hex_to_rgb(hex_code, mode='sheets'):
+    hex_code = hex_code.lstrip('#')
+    rgb = tuple(int(hex_code[i:i+2], 16) for i in (0, 2, 4))
+    if mode == 'sheets':
+        return {i: v / 255 for i, v in zip(['red', 'green', 'blue'], rgb)}
+    else:
+        return rgb
```

### Comparing `core_pro-0.0.8/src/core_pro/GSlide.py` & `core_pro-0.0.9/src/core_pro/GSlide.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from colorama import Fore
-from collections import defaultdict
-from .config import GoogleAuthentication
-from .GDrive import Drive
-
-
-class Slide(GoogleAuthentication):
-    service_type = 'slides'
-
-    def __init__(self, presentationId: str, service_type=service_type):
-        super().__init__(service_type)
-        self.pre_id = presentationId
-        self.status = f'{Fore.LIGHTYELLOW_EX}🐱 Slides:{Fore.RESET}'
-        self.all_info = self.service.presentations().get(presentationId=self.pre_id).execute().get('slides')
-        self.slide_idx = {idx: slide.get('objectId') for idx, slide in enumerate(self.all_info, start=1)}
-
-    def duplicate_slide(self, num_slide: int):
-        requests = [
-            {'duplicateObject': {'objectId': self.slide_idx.get(num_slide), 'objectIds': {}}}
-        ]
-        body = {'requests': requests}
-        self.service.presentations().batchUpdate(presentationId=self.pre_id, body=body).execute()
-        print(f'{self.status} duplicate slide {num_slide}')
-
-    def create_image(self, url: str, num_slide: int, size: dict, position: dict):
-        requests = [
-            {
-                'createImage': {
-                    'elementProperties': {
-                        'pageObjectId': self.slide_idx.get(num_slide),
-                        'size': size,
-                        'transform': position
-                    },
-                    'url': url
-                }
-            }
-        ]
-        body = {'requests': requests}
-        self.service.presentations().batchUpdate(presentationId=self.pre_id, body=body).execute()
-        print(f"{self.status} created a image at slide {num_slide}")
-
-    def delete_object(self, object_id):
-        requests = [{'deleteObject': {'objectId': object_id,}}]
-        body = {'requests': requests}
-        self.service.presentations().batchUpdate(presentationId=self.pre_id, body=body).execute()
-        print(f"{self.status} remove a object {object_id}")
-
-    def replace_images_by_drive(self, img_path, num_slide: int, size: dict, position: dict):
-        """drive folder_id is fixed"""
-        # upload by Drive
-        drive = Drive()
-        folder_id = '1jO-tbvoIyqeJcXD2EmgWSkSZMFc-fMCn'  # media folder
-        file_upload = drive.upload(file_dir=img_path, name_on_drive='test', folder_id=folder_id)
-        file_upload_id = file_upload.get('id')
-
-        # permission
-        drive.share_publicly(file_id=file_upload_id)
-        url = f"https://drive.google.com/uc?export=view&id={file_upload_id}"
-        self.create_image(url=url, num_slide=num_slide, size=size, position=position)
-
-        # remove permission
-        drive.remove_share_publicly(file_upload_id)
-        print(f"{self.status} replace a image at slide {num_slide}")
-
-    def get_slide_object_image(self, num_slide):
-        img_dict = defaultdict(dict)
-        info = self.all_info[num_slide - 1]
-        for i in info.get('pageElements'):
-            objectid = i.get('objectId')
-            position = i.get('transform')
-            size = i.get('size')
-            if img_url := i.get('image', {}).get('contentUrl'):
-                img_dict[objectid].update({'url': img_url, 'position': position, 'size': size})
-        print(f"{self.status} get image objects at slide {num_slide}")
-        return img_dict
+from colorama import Fore
+from collections import defaultdict
+from .config import GoogleAuthentication
+from .GDrive import Drive
+
+
+class Slide(GoogleAuthentication):
+    service_type = 'slides'
+
+    def __init__(self, presentationId: str, service_type=service_type):
+        super().__init__(service_type)
+        self.pre_id = presentationId
+        self.status = f'{Fore.LIGHTYELLOW_EX}🐱 Slides:{Fore.RESET}'
+        self.all_info = self.service.presentations().get(presentationId=self.pre_id).execute().get('slides')
+        self.slide_idx = {idx: slide.get('objectId') for idx, slide in enumerate(self.all_info, start=1)}
+
+    def duplicate_slide(self, num_slide: int):
+        requests = [
+            {'duplicateObject': {'objectId': self.slide_idx.get(num_slide), 'objectIds': {}}}
+        ]
+        body = {'requests': requests}
+        self.service.presentations().batchUpdate(presentationId=self.pre_id, body=body).execute()
+        print(f'{self.status} duplicate slide {num_slide}')
+
+    def create_image(self, url: str, num_slide: int, size: dict, position: dict):
+        requests = [
+            {
+                'createImage': {
+                    'elementProperties': {
+                        'pageObjectId': self.slide_idx.get(num_slide),
+                        'size': size,
+                        'transform': position
+                    },
+                    'url': url
+                }
+            }
+        ]
+        body = {'requests': requests}
+        self.service.presentations().batchUpdate(presentationId=self.pre_id, body=body).execute()
+        print(f"{self.status} created a image at slide {num_slide}")
+
+    def delete_object(self, object_id):
+        requests = [{'deleteObject': {'objectId': object_id,}}]
+        body = {'requests': requests}
+        self.service.presentations().batchUpdate(presentationId=self.pre_id, body=body).execute()
+        print(f"{self.status} remove a object {object_id}")
+
+    def replace_images_by_drive(self, img_path, num_slide: int, size: dict, position: dict):
+        """drive folder_id is fixed"""
+        # upload by Drive
+        drive = Drive()
+        folder_id = '1jO-tbvoIyqeJcXD2EmgWSkSZMFc-fMCn'  # media folder
+        file_upload = drive.upload(file_dir=img_path, name_on_drive='test', folder_id=folder_id)
+        file_upload_id = file_upload.get('id')
+
+        # permission
+        drive.share_publicly(file_id=file_upload_id)
+        url = f"https://drive.google.com/uc?export=view&id={file_upload_id}"
+        self.create_image(url=url, num_slide=num_slide, size=size, position=position)
+
+        # remove permission
+        drive.remove_share_publicly(file_upload_id)
+        print(f"{self.status} replace a image at slide {num_slide}")
+
+    def get_slide_object_image(self, num_slide):
+        img_dict = defaultdict(dict)
+        info = self.all_info[num_slide - 1]
+        for i in info.get('pageElements'):
+            objectid = i.get('objectId')
+            position = i.get('transform')
+            size = i.get('size')
+            if img_url := i.get('image', {}).get('contentUrl'):
+                img_dict[objectid].update({'url': img_url, 'position': position, 'size': size})
+        print(f"{self.status} get image objects at slide {num_slide}")
+        return img_dict
```

### Comparing `core_pro-0.0.8/src/core_pro/cloud.py` & `core_pro-0.0.9/src/core_pro/cloud.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import boto3
-import os
-from colorama import Fore
-from pathlib import Path
-from tqdm import tqdm
-from google.cloud import storage
-import datetime
-
-
-class AWS:
-    def __init__(self, bucket_name: str):
-        dict_ = {
-            'endpoint_url': 'https://s3g.data-infra.shopee.io',
-            'aws_access_key_id': os.environ['PRESTO_USER'],
-            'aws_secret_access_key': os.environ['PRESTO_PASSWORD'],
-        }
-        self.bucket_name = bucket_name
-        self.client = boto3.client('s3', **dict_)
-        self.my_bucket = boto3.resource('s3', **dict_).Bucket(self.bucket_name)
-        self.status = f'{Fore.LIGHTCYAN_EX}🐸 S3:{Fore.RESET}'
-
-    def get_file_size(self, key: str):
-        return self.my_bucket.Object(key).content_length
-
-    def upload_file(self, file: Path):
-        file_size = file.stat().st_size
-        with tqdm(total=file_size, unit='B', unit_scale=True, desc=f'Upload - {file.name}') as pbar:
-            self.my_bucket.upload_file(
-                file,
-                Key=file.stem,
-                Callback=lambda x: pbar.update(x))
-        print(f'{self.status} Upload file successfully')
-
-    def download_file(self, path: Path, key: str):
-        file_size = self.get_file_size(key)
-        with tqdm(total=file_size, unit="B", unit_scale=True, desc=f'Download - {key}') as pbar:
-            self.my_bucket.download_file(
-                Key=key,
-                Filename=path / key,
-                Callback=lambda x: pbar.update(x),
-            )
-        print(f'{self.status} Download file successfully')
-
-    def create_presigned_url(self, key: str, expiration: int = 900):
-        url = self.client.generate_presigned_url(
-            'get_object',
-            Params={'Bucket': self.bucket_name, 'Key': key},
-            ExpiresIn=expiration
-        )
-        print(f'{self.status} Presigned [{key}] in {expiration / 3600}h')
-        return url
-
-
-class Gcloud:
-    def __init__(self, json_path: str):
-        path = Path.home() / json_path
-        self.client = storage.Client.from_service_account_json(str(path))
-        self.status = f'{Fore.LIGHTBLUE_EX}🐻‍❄️ Gcloud:{Fore.RESET}'
-        self.bucket_name = 'kevin-bi'
-        self.bucket = self.client.bucket(self.bucket_name)
-
-    def download_file(self, blob_path: str, file_path: Path):
-        blob = self.bucket.blob(blob_path)
-        blob.download_to_filename(file_path)
-        print(f'{self.status} download {blob_path}')
-
-    def upload_file(self, blob_path: str, file_path: Path):
-        blob_path_full = f'{blob_path}/{file_path.name}'
-        blob = self.bucket.blob(blob_path_full)
-        blob.upload_from_filename(file_path)
-        print(f'{self.status} upload {file_path.stem} to {blob_path}')
-        return blob_path_full
-
-    def generate_download_signed_url_v4(self, blob_file, minutes=15):
-        blob = self.bucket.blob(blob_file)
-        url = blob.generate_signed_url(
-            version='v4',
-            expiration=datetime.timedelta(minutes=minutes),
-            method='GET',
-            response_type='image/png',
-        )
-        print(f'{self.status} Presigned [{blob_file}] in {minutes} mins')
-        return url
+import boto3
+import os
+from colorama import Fore
+from pathlib import Path
+from tqdm import tqdm
+from google.cloud import storage
+import datetime
+
+
+class AWS:
+    def __init__(self, bucket_name: str):
+        dict_ = {
+            'endpoint_url': 'https://s3g.data-infra.shopee.io',
+            'aws_access_key_id': os.environ['PRESTO_USER'],
+            'aws_secret_access_key': os.environ['PRESTO_PASSWORD'],
+        }
+        self.bucket_name = bucket_name
+        self.client = boto3.client('s3', **dict_)
+        self.my_bucket = boto3.resource('s3', **dict_).Bucket(self.bucket_name)
+        self.status = f'{Fore.LIGHTCYAN_EX}🐸 S3:{Fore.RESET}'
+
+    def get_file_size(self, key: str):
+        return self.my_bucket.Object(key).content_length
+
+    def upload_file(self, file: Path):
+        file_size = file.stat().st_size
+        with tqdm(total=file_size, unit='B', unit_scale=True, desc=f'Upload - {file.name}') as pbar:
+            self.my_bucket.upload_file(
+                file,
+                Key=file.stem,
+                Callback=lambda x: pbar.update(x))
+        print(f'{self.status} Upload file successfully')
+
+    def download_file(self, path: Path, key: str):
+        file_size = self.get_file_size(key)
+        with tqdm(total=file_size, unit="B", unit_scale=True, desc=f'Download - {key}') as pbar:
+            self.my_bucket.download_file(
+                Key=key,
+                Filename=path / key,
+                Callback=lambda x: pbar.update(x),
+            )
+        print(f'{self.status} Download file successfully')
+
+    def create_presigned_url(self, key: str, expiration: int = 900):
+        url = self.client.generate_presigned_url(
+            'get_object',
+            Params={'Bucket': self.bucket_name, 'Key': key},
+            ExpiresIn=expiration
+        )
+        print(f'{self.status} Presigned [{key}] in {expiration / 3600}h')
+        return url
+
+
+class Gcloud:
+    def __init__(self, json_path: str):
+        path = Path.home() / json_path
+        self.client = storage.Client.from_service_account_json(str(path))
+        self.status = f'{Fore.LIGHTBLUE_EX}🐻‍❄️ Gcloud:{Fore.RESET}'
+        self.bucket_name = 'kevin-bi'
+        self.bucket = self.client.bucket(self.bucket_name)
+
+    def download_file(self, blob_path: str, file_path: Path):
+        blob = self.bucket.blob(blob_path)
+        blob.download_to_filename(file_path)
+        print(f'{self.status} download {blob_path}')
+
+    def upload_file(self, blob_path: str, file_path: Path):
+        blob_path_full = f'{blob_path}/{file_path.name}'
+        blob = self.bucket.blob(blob_path_full)
+        blob.upload_from_filename(file_path)
+        print(f'{self.status} upload {file_path.stem} to {blob_path}')
+        return blob_path_full
+
+    def generate_download_signed_url_v4(self, blob_file, minutes=15):
+        blob = self.bucket.blob(blob_file)
+        url = blob.generate_signed_url(
+            version='v4',
+            expiration=datetime.timedelta(minutes=minutes),
+            method='GET',
+            response_type='image/png',
+        )
+        print(f'{self.status} Presigned [{blob_file}] in {minutes} mins')
+        return url
```

### Comparing `core_pro-0.0.8/src/core_pro/config.py` & `core_pro-0.0.9/src/core_pro/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,66 @@
-import pickle
-from pathlib import Path
-from googleapiclient.discovery import build
-from google_auth_oauthlib.flow import InstalledAppFlow
-from google.auth.transport.requests import Request
-
-google_services = {
-    'sheets': {
-        'scopes': ['https://www.googleapis.com/auth/spreadsheets'],
-        'versions': 'v4',
-    },
-    'gmail': {
-        'scopes': ['https://mail.google.com/'],
-        'versions': 'v1',
-    },
-    'drive': {
-        'scopes': ['https://www.googleapis.com/auth/drive'],
-        'versions': 'v3',
-    },
-    'slides': {
-        'scopes': ['https://www.googleapis.com/auth/presentations'],
-        'versions': 'v1',
-    }
-}
-
-
-class GoogleAuthentication:
-
-    def __init__(self, service_type: str):
-        """
-        get google credentials
-        :param service_type: 'sheets', 'gmail or 'drive' services
-        :return: google credential
-        """
-        creds = None
-        scopes, versions = google_services[service_type].values()
-
-        # find project path
-        lst_path = [*Path.cwd().parents]
-        project_path = lst_path[0]
-        for i, v in enumerate(lst_path):
-            if v.parts[-1] in ['PycharmProjects']:
-                break
-            project_path = v
-
-        # define path
-        token_path = project_path / 'token'
-        token_name = token_path / f'token_{service_type}.pickle'
-        json_path = project_path / 'token_json/client_secret.json'
-        # check json
-        if not json_path.exists():
-            message = (
-                f"Please copy your json to the folder with name: 'client_secret.json'\n"
-                f"Path: {project_path / 'token_json'}"
-            )
-            raise Exception(message)
-        # create folder
-        if not token_path.exists():
-            token_path.mkdir(parents=True, exist_ok=True)
-        # check token
-        if token_name.exists():
-            creds = pickle.load(open(token_name, 'rb'))
-        if not creds or not creds.valid:
-            if creds and creds.expired and creds.refresh_token:
-                creds.refresh(Request())
-            else:
-                flow = InstalledAppFlow.from_client_secrets_file(str(json_path), scopes)
-                creds = flow.run_local_server(port=0)
-            pickle.dump(creds, open(token_name, 'wb'))
-
-        self.service = build(service_type, versions, credentials=creds)
+import pickle
+import os
+from pathlib import Path
+from googleapiclient.discovery import build
+from google_auth_oauthlib.flow import InstalledAppFlow
+from google.auth.transport.requests import Request
+
+google_services = {
+    'sheets': {
+        'scopes': ['https://www.googleapis.com/auth/spreadsheets'],
+        'versions': 'v4',
+    },
+    'gmail': {
+        'scopes': ['https://mail.google.com/'],
+        'versions': 'v1',
+    },
+    'drive': {
+        'scopes': ['https://www.googleapis.com/auth/drive', 'https://www.googleapis.com/auth/drive.readonly'],
+        'versions': 'v3',
+    },
+    'slides': {
+        'scopes': ['https://www.googleapis.com/auth/presentations'],
+        'versions': 'v1',
+    }
+}
+
+
+class GoogleAuthentication:
+
+    def __init__(self, service_type: str):
+        """
+        get google credentials
+        :param service_type: 'sheets', 'gmail or 'drive' services
+        :return: google credential
+        """
+        creds = None
+        scopes, versions = google_services[service_type].values()
+        project_path = Path(os.getenv('CRED_GG_API'))
+
+        # define path
+        token_path = project_path / 'token'
+        token_name = token_path / f'token_{service_type}.pickle'
+        json_path = project_path / 'token_json/client_secret.json'
+        # check json
+        if not json_path.exists():
+            message = (
+                f"Please set path in CRED_GG_API env "
+                f"and copy your json 'client_secret.json' to the folder: "
+                f"<CRED_GG_API>/token_json"
+            )
+            raise Exception(message)
+        # create folder
+        if not token_path.exists():
+            token_path.mkdir(parents=True, exist_ok=True)
+        # check token
+        if token_name.exists():
+            creds = pickle.load(open(token_name, 'rb'))
+        if not creds or not creds.valid:
+            if creds and creds.expired and creds.refresh_token:
+                creds.refresh(Request())
+            else:
+                flow = InstalledAppFlow.from_client_secrets_file(str(json_path), scopes)
+                creds = flow.run_local_server(port=0)
+            pickle.dump(creds, open(token_name, 'wb'))
+
+        self.service = build(service_type, versions, credentials=creds)
```

### Comparing `core_pro-0.0.8/src/core_pro/ultilities.py` & `core_pro-0.0.9/src/core_pro/ultilities.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from .GSheet import Sheet
-from datetime import timedelta, datetime
-from pathlib import Path
-import polars as pl
-import psutil
-from openpyxl.utils.cell import get_column_letter, column_index_from_string, coordinate_from_string
-
-
-def update_df(df, sheet_name: str, sheet_id: str, start: str = 'A1'):
-    # Call sheet
-    sheet = Sheet(sheet_id)
-    # Dataframe type
-    if isinstance(df, pl.DataFrame):
-        col_df = [*df.schema.keys()]
-        values = [col_df]
-        values.extend(df.to_pandas().astype(str).to_numpy().tolist())
-    else:
-        col_df = df.columns
-        values = df.transpose().reset_index().transpose().to_numpy().astype(str).tolist()
-    # Export to sheets
-    end = get_column_letter(len(col_df) + column_index_from_string(coordinate_from_string(start)[0]) - 1)
-    sheet.clear_gsheet(sheet_name, sheet_range=f"{start}:{end}")
-    sheet.update_value_single_axis(sheet_range=f"{start}:{end}", values=values,
-                                   sheet_name=sheet_name, value_input='USER_ENTERED')
-
-
-def format_df(sheet_name: str, sheet_id: str, num_col: int, start: str = 'A1'):
-    # Sheet
-    sheet = Sheet(sheet_id)
-    ws_id = sheet.get_worksheet_properties(sheet_name)['sheetId']
-    # Frozen
-    sheet.frozen_view(ws_id)
-    # Title
-    sheet.format_title(ws_id, start)
-    # Header
-    next_start = ''.join((coordinate_from_string(start)[0], str(coordinate_from_string(start)[1] + 1)))
-    sheet.format_header(ws_id, next_start, num_col)
-
-
-def make_dir(folder_name):
-    if not folder_name.exists():
-        folder_name.mkdir(parents=True, exist_ok=True)
-
-
-def update_stt(stt: str, pos: int, sheet_id: str, sheet_name: str):
-    Sheet(sheet_id).update_value_single_axis(sheet_range=f'I{pos}', sheet_name=sheet_name, values=stt)
-
-
-def remove_old_file(path, days: int, file_type: str):
-    check_date = datetime.today().date() - timedelta(days=days)
-    print(f'Files {file_type} before {check_date} ({days} days) will be removed')
-
-    for file in Path(path).glob(f'*.{file_type}'):
-        mdate = datetime.fromtimestamp(file.stat().st_mtime).date()
-        if mdate < check_date:
-            print(f'Remove: file {file.name} - mdate: {mdate}')
-            file.unlink()
-
-
-def memory_used(old: int = 0):
-    mem = psutil.Process().memory_full_info().uss / (1024 ** 2)
-    print(f"After {old:,.0f}MB memory is used: {mem - old:,.0f} MB, current: {mem:,.0f} MB")
-    return mem
+from .GSheet import Sheet
+from datetime import timedelta, datetime
+from pathlib import Path
+import polars as pl
+import psutil
+from openpyxl.utils.cell import get_column_letter, column_index_from_string, coordinate_from_string
+
+
+def update_df(df, sheet_name: str, sheet_id: str, start: str = 'A1'):
+    # Call sheet
+    sheet = Sheet(sheet_id)
+    # Dataframe type
+    if isinstance(df, pl.DataFrame):
+        col_df = [*df.schema.keys()]
+        values = [col_df]
+        values.extend(df.to_pandas().astype(str).to_numpy().tolist())
+    else:
+        col_df = df.columns
+        values = df.transpose().reset_index().transpose().to_numpy().astype(str).tolist()
+    # Export to sheets
+    end = get_column_letter(len(col_df) + column_index_from_string(coordinate_from_string(start)[0]) - 1)
+    sheet.clear_gsheet(sheet_name, sheet_range=f"{start}:{end}")
+    sheet.update_value_single_axis(sheet_range=f"{start}:{end}", values=values,
+                                   sheet_name=sheet_name, value_input='USER_ENTERED')
+
+
+def format_df(sheet_name: str, sheet_id: str, num_col: int, start: str = 'A1'):
+    # Sheet
+    sheet = Sheet(sheet_id)
+    ws_id = sheet.get_worksheet_properties(sheet_name)['sheetId']
+    # Frozen
+    sheet.frozen_view(ws_id)
+    # Title
+    sheet.format_title(ws_id, start)
+    # Header
+    next_start = ''.join((coordinate_from_string(start)[0], str(coordinate_from_string(start)[1] + 1)))
+    sheet.format_header(ws_id, next_start, num_col)
+
+
+def make_dir(folder_name):
+    if not folder_name.exists():
+        folder_name.mkdir(parents=True, exist_ok=True)
+
+
+def update_stt(stt: str, pos: int, sheet_id: str, sheet_name: str):
+    Sheet(sheet_id).update_value_single_axis(sheet_range=f'I{pos}', sheet_name=sheet_name, values=stt)
+
+
+def remove_old_file(path, days: int, file_type: str):
+    check_date = datetime.today().date() - timedelta(days=days)
+    print(f'Files {file_type} before {check_date} ({days} days) will be removed')
+
+    for file in Path(path).glob(f'*.{file_type}'):
+        mdate = datetime.fromtimestamp(file.stat().st_mtime).date()
+        if mdate < check_date:
+            print(f'Remove: file {file.name} - mdate: {mdate}')
+            file.unlink()
+
+
+def memory_used(old: int = 0):
+    mem = psutil.Process().memory_full_info().uss / (1024 ** 2)
+    print(f"After {old:,.0f}MB memory is used: {mem - old:,.0f} MB, current: {mem:,.0f} MB")
+    return mem
```

### Comparing `core_pro-0.0.8/LICENSE` & `core_pro-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2023 Kevin Khang
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2023 Kevin Khang
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `core_pro-0.0.8/pyproject.toml` & `core_pro-0.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "core_pro"
-version = "0.0.8"
-authors = [
-  { name="Kevin Khang", email="kevinkhang2909@gmail.com" },
-]
-description = "A utility package for data science"
-readme = "README.md"
-requires-python = ">=3.9"
-license = {file = "LICENSE"}
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-keywords = ["api, google, aws"]
-dependencies = [
-    'func-timeout',
-    'google-api-python-client',
-    'google-auth-oauthlib',
-    'tqdm',
-    'sqlalchemy',
-    'pyarrow',
-    'trino',
-    'openpyxl',
-    'colorama',
-    'boto3',
-    'polars',
-    'pandas',
-    'google-cloud-storage',
-]
-
-[project.urls]
-"Homepage" = "https://github.com/kevinkhang2909/core_pro"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "core_pro"
+version = "0.0.9"
+authors = [
+  { name="Kevin Khang", email="kevinkhang2909@gmail.com" },
+]
+description = "A utility package for data science"
+readme = "README.md"
+requires-python = ">=3.9"
+license = {file = "LICENSE"}
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+keywords = ["api, google, aws"]
+dependencies = [
+    'func-timeout',
+    'google-api-python-client',
+    'google-auth-oauthlib',
+    'tqdm',
+    'sqlalchemy',
+    'pyarrow',
+    'trino',
+    'openpyxl',
+    'colorama',
+    'boto3',
+    'polars',
+    'pandas',
+    'google-cloud-storage',
+]
+
+[project.urls]
+"Homepage" = "https://github.com/kevinkhang2909/core_pro"
 "Bug Tracker" = "https://github.com/kevinkhang2909/core_pro/issues"
```

### Comparing `core_pro-0.0.8/PKG-INFO` & `core_pro-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core_pro
-Version: 0.0.8
+Version: 0.0.9
 Summary: A utility package for data science
 Project-URL: Homepage, https://github.com/kevinkhang2909/core_pro
 Project-URL: Bug Tracker, https://github.com/kevinkhang2909/core_pro/issues
 Author-email: Kevin Khang <kevinkhang2909@gmail.com>
 License: Copyright (c) 2023 Kevin Khang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

