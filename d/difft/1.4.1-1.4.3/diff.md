# Comparing `tmp/difft-1.4.1-py3-none-any.whl.zip` & `tmp/difft-1.4.3-py2-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 12433 bytes, number of entries: 14
+Zip file size: 12916 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-30 08:05 difft/__init__.py
--rw-r--r--  2.0 unx     1393 b- defN 23-Jan-30 08:05 difft/attachment.py
--rw-r--r--  2.0 unx     3131 b- defN 23-Dec-18 09:01 difft/auth.py
--rw-r--r--  2.0 unx    14464 b- defN 23-Dec-18 09:01 difft/client.py
+-rw-r--r--  2.0 unx     1358 b- defN 24-Mar-28 11:35 difft/attachment.py
+-rw-r--r--  2.0 unx     3101 b- defN 24-Mar-28 11:35 difft/auth.py
+-rw-r--r--  2.0 unx    13365 b- defN 24-Mar-28 11:35 difft/client.py
 -rw-r--r--  2.0 unx     7741 b- defN 23-Jan-30 08:05 difft/command.py
 -rw-r--r--  2.0 unx      700 b- defN 23-Dec-18 09:01 difft/constants.py
+-rw-r--r--  2.0 unx     1907 b- defN 24-Mar-28 11:35 difft/crypto.py
 -rw-r--r--  2.0 unx     3802 b- defN 23-Dec-18 09:01 difft/difft_ws_listener.py
--rw-r--r--  2.0 unx     3140 b- defN 23-Dec-18 09:01 difft/message.py
--rw-r--r--  2.0 unx     1588 b- defN 23-Dec-18 09:01 difft/utils.py
--rw-r--r--  2.0 unx      327 b- defN 23-Dec-18 10:14 difft-1.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-18 10:14 difft-1.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Dec-18 10:14 difft-1.4.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Dec-18 10:14 difft-1.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1045 b- defN 23-Dec-18 10:14 difft-1.4.1.dist-info/RECORD
-14 files, 37479 bytes uncompressed, 10723 bytes compressed:  71.4%
+-rw-r--r--  2.0 unx     3059 b- defN 24-Mar-28 11:35 difft/message.py
+-rw-r--r--  2.0 unx     1598 b- defN 24-Mar-28 11:35 difft/utils.py
+-rw-r--r--  2.0 unx      327 b- defN 24-Apr-01 10:30 difft-1.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 10:30 difft-1.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 24-Apr-01 10:30 difft-1.4.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-01 10:30 difft-1.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1117 b- defN 24-Apr-01 10:30 difft-1.4.3.dist-info/RECORD
+15 files, 38223 bytes uncompressed, 11100 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -12,32 +12,35 @@
 
 Filename: difft/command.py
 Comment: 
 
 Filename: difft/constants.py
 Comment: 
 
+Filename: difft/crypto.py
+Comment: 
+
 Filename: difft/difft_ws_listener.py
 Comment: 
 
 Filename: difft/message.py
 Comment: 
 
 Filename: difft/utils.py
 Comment: 
 
-Filename: difft-1.4.1.dist-info/METADATA
+Filename: difft-1.4.3.dist-info/METADATA
 Comment: 
 
-Filename: difft-1.4.1.dist-info/WHEEL
+Filename: difft-1.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: difft-1.4.1.dist-info/entry_points.txt
+Filename: difft-1.4.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: difft-1.4.1.dist-info/top_level.txt
+Filename: difft-1.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: difft-1.4.1.dist-info/RECORD
+Filename: difft-1.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## difft/attachment.py

```diff
@@ -1,54 +1,54 @@
 class AttachmentBuilder:
     def __init__(self) -> None:
         self._attachment = dict(contentType="text/html")
-    
+
     def authorize_id(self, authorize_id):
         self._attachment["authorizeId"] = authorize_id
         return self
-    
+
     def key(self, key):
         self._attachment["key"] = key
         return self
-    
+
     def file_size(self, file_size):
         self._attachment["size"] = file_size
         return self
-    
+
     def file_name(self, file_name):
         self._attachment["fileName"] = file_name
         return self
-    
+
     def digest(self, cipher_hash):
         self._attachment["digest"] = cipher_hash
         return self
-    
+
     def content_type(self, content_type):
         self._attachment["contentType"] = content_type
         return self
-    
+
     def flags(self, flags):
         self._attachment["flags"] = flags
         return self
 
     def width(self, width):
         self._attachment["width"] = width
         return self
-    
+
     def height(self, height):
         self._attachment["height"] = height
         return self
 
     def preview(self, preview):
         self._attachment["preview"] = preview
         return self
 
     def caption(self, caption):
         self._attachment["caption"] = caption
         return self
-    
+
     def url(self, url):
         self._attachment["url"] = url
         return self
 
     def build(self):
-        return self._attachment
+        return self._attachment
```

## difft/auth.py

```diff
@@ -88,11 +88,10 @@
 
     def sign(self, msg: bytes) -> Signature:
         ts = current_milli_time()
         nonce = get_nonce()
         data = ";".join([self._appid, str(ts), nonce]) + ";"
         msg = data.encode("utf-8") + msg
         sign_str = hmac.new(self._key, msg, hashlib.sha256).hexdigest()
-        signature = Signature(
+        return Signature(
             timestamp=ts, nonce=nonce, algorithm=constants.ALGORITHM_HMAC_SHA256, signature=sign_str
         )
-        return signature
```

## difft/client.py

```diff
@@ -1,62 +1,82 @@
-import os
 import base64
 import hashlib
-import hmac
 import json
 import logging
+import os
 
 import requests
-from Crypto.Cipher import AES
-from Crypto.Random import get_random_bytes
 
 from difft import constants
-from difft.utils import parse_response
 from difft.auth import Authenticator
+from difft.crypto import decrypt_attachment, encrypt_attachment
+from difft.utils import parse_response
 
 
 class DifftClient:
-    BLOCK_SIZE = 16
+    """Main class wrapper around Wea methods.
+
+    Wraps authentication logic as well as some more complex workflows like
+    sendin medias.
+
+    """
+
+    # arbitrary that's high enough given my ignorance of the difft server, but
+    # small enough most API won't significantly break if we hit it
+    # not applied on media requests.
+    REQUEST_TIMEOUT = 5
 
     def __init__(self, appid: str, key: str, host: str = "https://openapi.test.difft.org"):
         self._auth = Authenticator(appid, key.encode("utf-8"))
         self._host = host
 
-    def upload_attachment(self, send_wuid: str, group_ids: list, acceptor_wuid: list, attachment: bytes) -> dict:
-        """
-        Upload attachment to oss storage
+    def upload_attachment(
+        self, send_wuid: str, group_ids: list, acceptor_wuid: list, attachment: bytes
+    ) -> dict:
+        """Upload attachment to oss storage.
+
         :param send_wuid: bot wuid
         :param group_ids: list of group id
         :param acceptor_wuid: list of acceptor wuid
         :param attachment: bytes of attachment
+
         :return: map of authorizeId, key, cipherHash, fileSize
         """
         key = hashlib.sha512(attachment).digest()
         fileHash = hashlib.sha256(key).digest()
         fileSize = len(attachment)
-        is_exist_body = dict(wuid=send_wuid, fileHash=base64.b64encode(fileHash).decode("utf-8"), fileSize=fileSize,
-                             gids=group_ids, numbers=acceptor_wuid)
-        is_exist_resp = requests.post(url=self._host + constants.URL_ISEXIST, json=is_exist_body, auth=self._auth)
+        is_exist_body = dict(
+            wuid=send_wuid,
+            fileHash=base64.b64encode(fileHash).decode("utf-8"),
+            fileSize=fileSize,
+            gids=group_ids,
+            numbers=acceptor_wuid,
+        )
+        is_exist_resp = requests.post(
+            url=self._host + constants.URL_ISEXIST,
+            json=is_exist_body,
+            auth=self._auth,
+        )
 
         is_exist_resp_obj = json.loads(is_exist_resp.text)
         if is_exist_resp_obj.get("status") != 0:
             raise Exception(is_exist_resp_obj.get("reason"))
 
         data = is_exist_resp_obj.get("data")
         if data.get("exists"):
             # file already exist, skip upload
             return dict(
                 authorizeId=data.get("authorizeId"),
                 key=base64.b64encode(key).decode("utf-8"),
                 cipherHash=data.get("cipherHash"),
-                fileSize=fileSize
+                fileSize=fileSize,
             )
 
         # upload attachment to oss
-        ciphertext = self.encrypt_attachment(attachment, key)
+        ciphertext = encrypt_attachment(attachment, key)
         cipherHash = hashlib.md5(ciphertext).hexdigest()
         requests.put(data.get("url"), data=ciphertext)
 
         upload_info = dict(
             wuid=send_wuid,
             fileHash=base64.b64encode(fileHash).decode("utf-8"),
             attachmentId=data.get("attachmentId"),
@@ -66,96 +86,115 @@
             encAlg="AES-CBC-SHA256",
             cipherHash=cipherHash,
             cipherHashType="MD5",
             gids=group_ids,
             numbers=acceptor_wuid,
         )
         # report uploadinfo to server
-        upload_info_resp = requests.post(url=self._host + constants.URL_UPLOAD_ATTACHMENT, json=upload_info,
-                                         auth=self._auth)
+        upload_info_resp = requests.post(
+            url=self._host + constants.URL_UPLOAD_ATTACHMENT, json=upload_info, auth=self._auth
+        )
         upload_info_resp_obj = json.loads(upload_info_resp.text)
         if upload_info_resp_obj.get("status") != 0:
             raise Exception(upload_info_resp_obj.get("reason"))
         data = upload_info_resp_obj.get("data")
         return dict(
             authorizeId=data.get("authorizeId"),
             key=base64.b64encode(key).decode("utf-8"),
             cipherHash=cipherHash,
-            fileSize=fileSize
+            fileSize=fileSize,
         )
 
     def download_attachment(self, wuid, key, authorize_id, cipher_hash, url=None) -> bytes:
-        """
-        Download attachment from oss
+        """Download attachment from oss.
+
         :param wuid: bot id
         :param key:
         :param authorize_id:
         :param cipher_hash:
         :param url: attachment download link if existed, default None
+
         :return: plain attachment, bytes
         """
         key = base64.b64decode(key)
         if not url:
             fileHash = hashlib.sha256(key).digest()
-            download_attachment_body = dict(wuid=wuid, fileHash=base64.b64encode(fileHash).decode("utf-8"),
-                                            authorizeId=authorize_id)
-            download_attachment_resp = requests.post(url=self._host + constants.URL_DOWNLOAD_ATTACHMENT,
-                                                     json=download_attachment_body, auth=self._auth)
+            download_attachment_body = dict(
+                wuid=wuid,
+                fileHash=base64.b64encode(fileHash).decode("utf-8"),
+                authorizeId=authorize_id,
+            )
+            download_attachment_resp = requests.post(
+                url=self._host + constants.URL_DOWNLOAD_ATTACHMENT,
+                json=download_attachment_body,
+                auth=self._auth,
+            )
             download_attachment_obj = json.loads(download_attachment_resp.text)
             if download_attachment_obj.get("status") != 0:
                 raise Exception(download_attachment_obj.get("reason"))
             data = download_attachment_obj.get("data")
             url = data.get("url")
         attachment_resp = requests.get(url=url)
         attachment = attachment_resp.content
-        return self.decrypt_attachment(attachment, key, bytes.fromhex(cipher_hash))
+
+        return decrypt_attachment(attachment, key, bytes.fromhex(cipher_hash))
 
     def append_attachment_authorization(self, wuid, fil_hash, file_size, group_ids, acceptor_wuid):
-        """
-        Append user authorization to existed attachment
+        """Append user authorization to existed attachment.
+
         :param wuid: bot id
         :param fil_hash:
         :param file_size:
         :param group_ids:
         :param acceptor_wuid:
+
         :return: authorizeId if success, otherwise raise exception
         """
-        is_exist_body = dict(wuid=wuid, fileHash=fil_hash, fileSize=file_size, gids=group_ids, numbers=acceptor_wuid)
-        is_exist_resp = requests.post(url=self._host + constants.URL_ISEXIST, json=is_exist_body, auth=self._auth)
+        is_exist_body = dict(
+            wuid=wuid, fileHash=fil_hash, fileSize=file_size, gids=group_ids, numbers=acceptor_wuid
+        )
+        is_exist_resp = requests.post(
+            url=self._host + constants.URL_ISEXIST, json=is_exist_body, auth=self._auth
+        )
         is_exist_resp_obj = json.loads(is_exist_resp.text)
         if is_exist_resp_obj.get("status") != 0:
             raise Exception(is_exist_resp_obj.get("reason"))
 
         data = is_exist_resp_obj.get("data")
         if not data.get("exists"):
             raise Exception("file not exist")
 
         return data.get("authorizeId")
 
     def delete_attachment_authorization(self, wuid, filehash, authorizeIds):
-        """
-        Delete specific authorization by authorizeIds
+        """Delete specific authorization by authorizeIds,
+
         :param wuid:
         :param filehash:
         :param authorizeIds:
+
         :return: True if success
         """
-        delete_attachment_auth_body = dict(wuid=wuid,
-                                           delAuthorizeInfos=[dict(fileHash=filehash, authorizeIds=authorizeIds)])
-        delete_attachment_auth_resp = requests.post(url=self._host + constants.URL_DEL_ATTACHMENT,
-                                                    json=delete_attachment_auth_body, auth=self._auth)
+        delete_attachment_auth_body = dict(
+            wuid=wuid, delAuthorizeInfos=[dict(fileHash=filehash, authorizeIds=authorizeIds)]
+        )
+        delete_attachment_auth_resp = requests.post(
+            url=self._host + constants.URL_DEL_ATTACHMENT,
+            json=delete_attachment_auth_body,
+            auth=self._auth,
+        )
         delete_attachment_auth_obj = json.loads(delete_attachment_auth_resp.text)
         if delete_attachment_auth_obj.get("status") != 0:
             logging.error(delete_attachment_auth_obj.get("reason"))
             return False
         return True
 
     def upload_pic(self, picture_path, raw_response=False):
-        """
-        Upload picture so we can refer to it within messages.
+        """Upload picture so we can refer to it within messages.
+
         :param picture_path: any filename
         :return: online image url
                  {
                       "ver": 1,
                       "status": 0,
                       "reason": "success",
                       "data": {
@@ -167,38 +206,41 @@
             raise Exception("file %s not found" % picture_path)
 
         filename = os.path.basename(picture_path)
 
         with open(picture_path, "rb") as fd:
             content = base64.b64encode(fd.read())
 
-        payload ={
+        payload = {
             'file_name': filename,
             # make it serializable to json
             'content': content.decode('utf-8'),
         }
-        res = requests.post(url=self._host + constants.URL_UPLOAD_PIC, json=payload, auth=self._auth)
+        res = requests.post(
+            url=self._host + constants.URL_UPLOAD_PIC, json=payload, auth=self._auth
+        )
         if res.status_code != 200:
             raise Exception("failed to upload image, server responded with %d" % res.status_code)
         envelope = res.json()
         if envelope.get("status") != 0:
             raise Exception("pic upload failed", envelope.get("errors"), envelope.get("error"))
 
         # done managing error cases, send back data
         if raw_response:
             return envelope
         else:
             return envelope.get("data").get("url")
 
     def send_message(self, msg, raw_response=False):
-        """
-        Send message
+        """Send message.
+
         :param msg: MessageRequest
         :param raw_response: whether to get raw response or not
-        :return: list of fail reason, 
+
+        :return: list of fail reason,
                 [
                     {
                     "wuid":"idxxx",
                     "groupID":"{wea group id}",
                     "reason":"failed reason"
                     }
                 ]
@@ -209,20 +251,29 @@
                         "wuid":"idxxx",
                         "groupID":"{wea group id}",
                         "reason":"failed reason"
                     }],
                     "refID":"v1:1649814691000:+800000000" // 当消息可被引用时，返回该消息的refID
                 }
         """
-        send_msg_resp = requests.post(url=self._host + constants.URL_SEND_MSG, json=msg, auth=self._auth)
+        send_msg_resp = requests.post(
+            url=self._host + constants.URL_SEND_MSG,
+            json=msg,
+            auth=self._auth,
+            timeout=self.REQUEST_TIMEOUT,
+        )
         if send_msg_resp.status_code != 200:
             raise Exception("server response %d" % send_msg_resp.status_code)
         send_msg_resp_obj = json.loads(send_msg_resp.text)
         if send_msg_resp_obj.get("status") != 0:
-            raise Exception("send message failed", send_msg_resp_obj.get("errors"), send_msg_resp_obj.get("error"))
+            raise Exception(
+                "send message failed",
+                send_msg_resp_obj.get("errors"),
+                send_msg_resp_obj.get("error"),
+            )
         if raw_response:
             return send_msg_resp_obj
         else:
             return send_msg_resp_obj.get("errors")
 
     def get_account_by_email(self, email):
         param = dict(email=email)
@@ -232,44 +283,64 @@
         # see https://git.toolsfdg.net/difftim/difft-sdk-python/issues/8
         # unlike retrieval by email, it seems retrieval by wuid requires to
         # specify the operator (i.e. the bot id)
         param = dict(wuid=wuid, operator=operator)
         return self.get_account(param)
 
     def get_account(self, params):
-        resp = requests.get(url=self._host + constants.URL_ACCOUNT, params=params, auth=self._auth)
+        resp = requests.get(
+            url=self._host + constants.URL_ACCOUNT,
+            params=params,
+            auth=self._auth,
+            timeout=self.REQUEST_TIMEOUT,
+        )
         if resp.status_code != 200:
             raise Exception("server response error, code", resp.status_code)
         resp_obj = json.loads(resp.text)
         if resp_obj.get("status") != 0:
             raise Exception(resp_obj.get("reason"))
         return resp_obj.get("data")
 
     def create_group(self, payload):
-        resp = requests.post(url=self._host + constants.URL_GROUP, json=payload, auth=self._auth)
+        resp = requests.post(
+            url=self._host + constants.URL_GROUP,
+            json=payload,
+            auth=self._auth,
+            timeout=self.REQUEST_TIMEOUT,
+        )
         if resp.status_code != 200:
             raise Exception("server response error, code", resp.status_code)
         resp_obj = json.loads(resp.text)
         if resp_obj.get("status") != 0:
             raise Exception(resp_obj.get("reason"))
         return resp_obj.get("data")
 
     def add_members(self, gid, operator, accounts):
         payload = {'gid': gid, 'operator': operator, 'accounts': accounts}
-        resp = requests.put(url=self._host + constants.URL_ADD_MEMBERS, json=payload, auth=self._auth)
+        resp = requests.put(
+            url=self._host + constants.URL_ADD_MEMBERS,
+            json=payload,
+            auth=self._auth,
+            timeout=self.REQUEST_TIMEOUT,
+        )
         if resp.status_code != 200:
             raise Exception("server response error, code", resp.status_code)
         resp_obj = json.loads(resp.text)
         if resp_obj.get("status") != 0:
             raise Exception(resp_obj.get("reason"))
         return resp_obj.get("data")
-    
+
     def get_group_by_botid(self, botid):
         params = dict(operator=botid)
-        resp = requests.get(url=self._host + constants.URL_GROUP, params=params, auth=self._auth)
+        resp = requests.get(
+            url=self._host + constants.URL_GROUP,
+            params=params,
+            auth=self._auth,
+            timeout=self.REQUEST_TIMEOUT,
+        )
         if resp.status_code != 200:
             raise Exception("server response error, code", resp.status_code)
         resp_obj = json.loads(resp.text)
         if resp_obj.get("status") != 0:
             raise Exception(resp_obj.get("reason"))
         if "groups" in resp_obj.get("data"):
             return resp_obj.get("data").get("groups")
@@ -279,66 +350,13 @@
     def get_group_members(self, botid, gid):
         """Fetch group members.
 
         API: https://documenter.getpostman.com/view/14311359/UVREmkXq#8953dbf9-1fb7-486b-81a5-1b58938218d9
 
         """
         params = dict(operator=botid, gid=gid)
-        return requests.get(url=self._host + constants.URL_GROUP_MEMBERS, params=params, auth=self._auth)
-
-    def encrypt_attachment(self, attachment, key):
-        if len(key) != 64:
-            raise Exception("got invalid length keys (%d bytes)" % len(key))
-
-        iv = get_random_bytes(16)
-        cipher = AES.new(key[:32], AES.MODE_CBC, iv)
-        attachment_cipher = cipher.encrypt(self.pkcs5_pad(attachment))
-        mac = self.hmac_sha256(key[32:], iv, attachment_cipher)
-        ciphertext = iv + attachment_cipher + mac
-
-        return ciphertext
-
-    def decrypt_attachment(self, ciphertext, keys, thier_digest) -> bytes:
-        if len(keys) != 64:
-            raise Exception("got invalid length keys")
-
-        ciphertext_length = len(ciphertext)
-        iv = ciphertext[:16]
-        mac = ciphertext[ciphertext_length - 32:]
-        attachment_cipher = ciphertext[16:ciphertext_length - 32]
-        calculated_mac = self.hmac_sha256(keys[32:], iv, attachment_cipher)
-        if mac != calculated_mac:
-            raise Exception("bad mac")
-        if len(thier_digest) != 16:
-            raise Exception("unknown digest")
-        calculated_digest = hashlib.md5(ciphertext).digest()
-        if calculated_digest != thier_digest:
-            raise Exception("digest not match")
-
-        cipher = AES.new(keys[:32], AES.MODE_CBC, iv)
-        attachment_cipher = cipher.decrypt(attachment_cipher)
-        return self.pkcs5_unpad(attachment_cipher)
-
-    def pkcs5_pad(self, s):
-        """
-        padding to blocksize according to PKCS #5
-        calculates the number of missing chars to BLOCK_SIZE and pads with
-        ord(number of missing chars)
-        @param s: string to pad
-        @type s: string
-        @rtype: string
-        """
-        padded = self.BLOCK_SIZE - len(s) % self.BLOCK_SIZE
-        return s + padded * chr(padded).encode("utf-8")
-
-    def pkcs5_unpad(self, s):
-        """
-        unpadding according to PKCS #5
-        @param s: string to unpad
-        @type s: string
-        @rtype: string
-        """
-        return s[0:-s[-1]]
-
-    def hmac_sha256(self, keys, iv, ciphertext):
-        digest = hmac.new(keys, iv + ciphertext, hashlib.sha256).digest()
-        return digest
+        return requests.get(
+            url=self._host + constants.URL_GROUP_MEMBERS,
+            params=params,
+            auth=self._auth,
+            timeout=self.REQUEST_TIMEOUT,
+        )
```

## difft/message.py

```diff
@@ -1,79 +1,76 @@
 from difft.utils import current_milli_time
 
+
 class MessageRequestBuilder:
     def __init__(self) -> None:
         self.message_request = dict(version=1, type='TEXT', timestamp=current_milli_time())
 
     def sender(self, sender):
         self.message_request.update(dict(src=sender))
         return self
-    
-    def to_user(self, wuid:list):
+
+    def to_user(self, wuid: list):
         if not isinstance(wuid, list):
             raise Exception("user must be type list")
-        dest = {
-            "wuid": wuid,
-            "type": "USER"
-            }
+        dest = {"wuid": wuid, "type": "USER"}
         self.message_request['dest'] = dest
         return self
-    
+
     def message(self, msg):
         if 'msg' in self.message_request:
             self.message_request['msg']['body'] = msg
         else:
             self.message_request['msg'] = {'body': msg}
         return self
-    
+
     def to_group(self, group_id):
-        dest = {
-            "groupID": group_id,
-            "type": "GROUP"
-            }
+        dest = {"groupID": group_id, "type": "GROUP"}
         self.message_request['dest'] = dest
         return self
-    
+
     def at_user(self, wuid: list):
         if not isinstance(wuid, list):
             raise Exception("at user must be type list")
         if 'msg' in self.message_request:
             self.message_request['msg']['atPersons'] = wuid
         else:
             self.message_request['msg'] = {'atPersons': wuid}
         return self
-    
+
     def timestamp_now(self):
         self.message_request['timestamp'] = current_milli_time()
         return self
 
     def attachment(self, attachment):
         if 'msg' in self.message_request:
             self.message_request['msg']['attachment'] = attachment
         else:
             self.message_request['msg'] = {'attachment': attachment}
         return self
-    
+
     def quote(self, refID, text):
         if 'msg' in self.message_request:
             self.message_request['msg']['quote'] = {'refID': refID, 'text': text}
         else:
             self.message_request['msg'] = {'quote': {'refID': refID, 'text': text}}
         return self
-    
+
     def type(self, msg_type):
         self.message_request['type'] = msg_type
         return self
 
     def recall(self, source, timestamp, refID=""):
         self.message_request['type'] = 'RECALL'
-        self.message_request['recall'] = dict(realSource=dict(source=source, sourceDevice=1, timestamp=timestamp), refID=refID)
+        self.message_request['recall'] = dict(
+            realSource=dict(source=source, sourceDevice=1, timestamp=timestamp), refID=refID
+        )
         return self
 
-    def card(self, appid, id, content,fixedWidth=False, creator=None, timestamp=None, height=None):
+    def card(self, appid, id, content, fixedWidth=False, creator=None, timestamp=None, height=None):
         self.message_request['type'] = 'CARD'
         self.message_request['card'] = dict(appID=appid, id=id, content=content)
         if fixedWidth:
             self.message_request['card']['fixedWidth'] = fixedWidth
         if creator:
             self.message_request['card']['creator'] = creator
         if timestamp:
@@ -85,9 +82,7 @@
     def forwarded(self, forwarded):
         self.message_request['type'] = 'FORWARD'
         self.message_request['forwarded'] = forwarded
         return self
 
     def build(self):
         return self.message_request
-
-
```

## difft/utils.py

```diff
@@ -1,27 +1,30 @@
 import json
 import random
-import uuid, time
-
+import time
+import uuid
 
 HTTP_OK = 200
 SERVER_STATUS_OK = 0
 LETTERS = "abcdefghijklmnopqrstuvwxyz0123456789"
 
 
 def random_str(n: int):
-    return ''.join(random.choice(LETTERS) for i in range(n))
+    return ''.join(random.choice(LETTERS) for _ in range(n))
+
 
 def get_nonce():
     new_uuid = uuid.uuid4()
     return new_uuid.hex
 
+
 def current_milli_time():
     return round(time.time() * 1000)
 
+
 def parse_response(func):
     """Decorator to parse standard Difft server response.
 
     Note that if nothing bad is detected, it will return response['data'], and
     assume json response. While this seems to be the expected behaviour
     across the board, it means the caller needs to know how to access the
     underlying data (i.e. instead of getting a list of members, one need gets
@@ -31,21 +34,23 @@
     boilerplate, and anyway expose the initial server response payload.
 
     One downside though is that if moving to a more typed python, the function
     and the decorator will be poorly informative, and may justidy a different
     approach. But at this stage this seems to be the most productive.
 
     """
+
     def __inner(*args, **kwargs):
         # api call
         resp = func(*args, **kwargs)
 
         if resp.status_code != HTTP_OK:
             raise Exception("server response error, code", resp.status_code, resp.text)
 
         resp_obj = json.loads(resp.text)
 
         if resp_obj.get("status") != SERVER_STATUS_OK:
             raise Exception(resp_obj.get("reason"))
 
         return resp_obj.get("data")
+
     return __inner
```

