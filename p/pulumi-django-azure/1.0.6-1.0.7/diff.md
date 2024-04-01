# Comparing `tmp/pulumi-django-azure-1.0.6.tar.gz` & `tmp/pulumi-django-azure-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi-django-azure-1.0.6.tar", last modified: Mon Mar 25 06:39:16 2024, max compression
+gzip compressed data, was "pulumi-django-azure-1.0.7.tar", last modified: Mon Apr  1 14:34:26 2024, max compression
```

## Comparing `pulumi-django-azure-1.0.6.tar` & `pulumi-django-azure-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 06:39:16.366622 pulumi-django-azure-1.0.6/
--rw-rw-rw-   0        0        0     1087 2023-12-31 15:16:09.000000 pulumi-django-azure-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     7884 2024-03-25 06:39:16.366622 pulumi-django-azure-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5987 2024-02-08 19:55:35.000000 pulumi-django-azure-1.0.6/README.md
--rw-rw-rw-   0        0        0     1193 2024-03-25 06:38:10.000000 pulumi-django-azure-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       93 2024-03-25 06:39:16.369914 pulumi-django-azure-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-25 06:39:16.320789 pulumi-django-azure-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-03-25 06:39:16.333516 pulumi-django-azure-1.0.6/src/pulumi_django_azure/
--rw-rw-rw-   0        0        0       63 2024-02-08 20:15:37.000000 pulumi-django-azure-1.0.6/src/pulumi_django_azure/__init__.py
--rw-rw-rw-   0        0        0    23156 2024-03-25 06:37:51.000000 pulumi-django-azure-1.0.6/src/pulumi_django_azure/django_deployment.py
-drwxrwxrwx   0        0        0        0 2024-03-25 06:39:16.365706 pulumi-django-azure-1.0.6/src/pulumi_django_azure.egg-info/
--rw-rw-rw-   0        0        0     7884 2024-03-25 06:39:16.000000 pulumi-django-azure-1.0.6/src/pulumi_django_azure.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-03-25 06:39:16.000000 pulumi-django-azure-1.0.6/src/pulumi_django_azure.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 06:39:16.000000 pulumi-django-azure-1.0.6/src/pulumi_django_azure.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-03-25 06:39:16.000000 pulumi-django-azure-1.0.6/src/pulumi_django_azure.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-25 06:39:16.000000 pulumi-django-azure-1.0.6/src/pulumi_django_azure.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 14:34:26.214536 pulumi-django-azure-1.0.7/
+-rw-rw-rw-   0        0        0     1087 2023-12-31 15:16:09.000000 pulumi-django-azure-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     8110 2024-04-01 14:34:26.214536 pulumi-django-azure-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6213 2024-04-01 14:34:04.000000 pulumi-django-azure-1.0.7/README.md
+-rw-rw-rw-   0        0        0     1193 2024-04-01 14:34:04.000000 pulumi-django-azure-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       93 2024-04-01 14:34:26.217527 pulumi-django-azure-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 14:34:26.166411 pulumi-django-azure-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 14:34:26.188881 pulumi-django-azure-1.0.7/src/pulumi_django_azure/
+-rw-rw-rw-   0        0        0       63 2024-02-08 20:15:37.000000 pulumi-django-azure-1.0.7/src/pulumi_django_azure/__init__.py
+-rw-rw-rw-   0        0        0    26607 2024-04-01 14:34:04.000000 pulumi-django-azure-1.0.7/src/pulumi_django_azure/django_deployment.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:34:26.213535 pulumi-django-azure-1.0.7/src/pulumi_django_azure.egg-info/
+-rw-rw-rw-   0        0        0     8110 2024-04-01 14:34:26.000000 pulumi-django-azure-1.0.7/src/pulumi_django_azure.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-04-01 14:34:26.000000 pulumi-django-azure-1.0.7/src/pulumi_django_azure.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:34:26.000000 pulumi-django-azure-1.0.7/src/pulumi_django_azure.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-01 14:34:26.000000 pulumi-django-azure-1.0.7/src/pulumi_django_azure.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-01 14:34:26.000000 pulumi-django-azure-1.0.7/src/pulumi_django_azure.egg-info/top_level.txt
```

### Comparing `pulumi-django-azure-1.0.6/LICENSE` & `pulumi-django-azure-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pulumi-django-azure-1.0.6/PKG-INFO` & `pulumi-django-azure-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-django-azure
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simply deployment of Django on Azure with Pulumi
 Author-email: Maarten Ureel <maarten@youreal.eu>
 License: MIT License
         
         Copyright (c) 2023 YouReal BV
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,14 +41,15 @@
 
 This project aims to make a simple Django deployment on Azure easier.
 
 To have a proper and secure environment, we need these components:
 * Storage account for media and static files
 * CDN endpoint in front with a domain name of our choosing
 * PostgreSQL server
+* Azure Communication Services to send e-mails
 * Webapp with multiple custom host names and managed SSL for the website itself
 * Webapp running pgAdmin
 
 ## Installation
 This package is published on PyPi, so you can just add pulumi-django-azure to your requirements file.
 
 To use a specific branch in your project, add to pyproject.toml dependencies:
@@ -97,14 +98,16 @@
 django.add_django_website(
     name="web",
     db_name="mywebsite",
     repository_url="git@gitlab.com:project/website.git",
     repository_branch="main",
     website_hosts=["example.com", "www.example.com"],
     django_settings_module="mywebsite.settings.production",
+    comms_data_location="europe",
+    comms_domains=["mydomain.com"],
 )
 
 django.add_database_administrator(
     object_id="a1b2c3....",
     user_name="user@example.com",
     tenant_id="a1b2c3....",
 )
@@ -116,14 +119,15 @@
 2. Configure the PostgreSQL server (create and grant permissions to role for your websites)
 3. Retrieve the deployment SSH key and configure your remote GIT repository with it
 4. Configure your CDN host (add the CNAME record)
 5. Configure your custom website domains (add CNAME/A record and TXT validation records)
 6. Re-deploy with custom hosts
 7. Re-deploy once more to enable HTTPS on website domains
 8. Manually activate HTTPS on the CDN host
+9. Go to the e-mail communications service on Azure and configure DKIM, SPF,... for your custom domains.
 
 ## Custom domain name for CDN
 When deploying the first time, you will get a `cdn_cname` output. You need to create a CNAME to this domain before the deployment of the custom domain will succeed.
 
 You can safely deploy with the failing CustomDomain to get the CNAME, create the record and then deploy again.
 
 To enable HTTPS, you need to do this manually in the console. This is because of a limitation in the Azure API:
```

### Comparing `pulumi-django-azure-1.0.6/README.md` & `pulumi-django-azure-1.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 This project aims to make a simple Django deployment on Azure easier.
 
 To have a proper and secure environment, we need these components:
 * Storage account for media and static files
 * CDN endpoint in front with a domain name of our choosing
 * PostgreSQL server
+* Azure Communication Services to send e-mails
 * Webapp with multiple custom host names and managed SSL for the website itself
 * Webapp running pgAdmin
 
 ## Installation
 This package is published on PyPi, so you can just add pulumi-django-azure to your requirements file.
 
 To use a specific branch in your project, add to pyproject.toml dependencies:
@@ -58,14 +59,16 @@
 django.add_django_website(
     name="web",
     db_name="mywebsite",
     repository_url="git@gitlab.com:project/website.git",
     repository_branch="main",
     website_hosts=["example.com", "www.example.com"],
     django_settings_module="mywebsite.settings.production",
+    comms_data_location="europe",
+    comms_domains=["mydomain.com"],
 )
 
 django.add_database_administrator(
     object_id="a1b2c3....",
     user_name="user@example.com",
     tenant_id="a1b2c3....",
 )
@@ -77,14 +80,15 @@
 2. Configure the PostgreSQL server (create and grant permissions to role for your websites)
 3. Retrieve the deployment SSH key and configure your remote GIT repository with it
 4. Configure your CDN host (add the CNAME record)
 5. Configure your custom website domains (add CNAME/A record and TXT validation records)
 6. Re-deploy with custom hosts
 7. Re-deploy once more to enable HTTPS on website domains
 8. Manually activate HTTPS on the CDN host
+9. Go to the e-mail communications service on Azure and configure DKIM, SPF,... for your custom domains.
 
 ## Custom domain name for CDN
 When deploying the first time, you will get a `cdn_cname` output. You need to create a CNAME to this domain before the deployment of the custom domain will succeed.
 
 You can safely deploy with the failing CustomDomain to get the CNAME, create the record and then deploy again.
 
 To enable HTTPS, you need to do this manually in the console. This is because of a limitation in the Azure API:
```

### Comparing `pulumi-django-azure-1.0.6/pyproject.toml` & `pulumi-django-azure-1.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pulumi-django-azure"
-version = "1.0.6"
+version = "1.0.7"
 description = "Simply deployment of Django on Azure with Pulumi"
 readme = "README.md"
 authors = [{ name = "Maarten Ureel", email = "maarten@youreal.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -23,15 +23,15 @@
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://gitlab.com/MaartenUreel/pulumi-django-azure"
 
 [tool.poetry]
 name = "pulumi-django-azure"
-version = "1.0.6"
+version = "1.0.7"
 description = "Simply deployment of Django on Azure with Pulumi"
 authors = ["Maarten Ureel <maarten@youreal.eu>"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pulumi-azure-native = "^2.24.0"
 pulumi = "^3.99.0"
```

### Comparing `pulumi-django-azure-1.0.6/src/pulumi_django_azure/django_deployment.py` & `pulumi-django-azure-1.0.7/src/pulumi_django_azure/django_deployment.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,19 +25,21 @@
         """
         Create a Django deployment.
 
         :param name: The name of the deployment, will be used to name subresources.
         :param tenant_id: The Entra tenant ID for the database authentication.
         :param resource_group_name: The resource group name to create the resources in.
         :param vnet: The virtual network to create the subnets in.
+        :param pgsql_sku: The SKU for the PostgreSQL server.
         :param pgsql_ip_prefix: The IP prefix for the PostgreSQL subnet.
         :param appservice_ip_prefix: The IP prefix for the app service subnet.
         :param app_service_sku: The SKU for the app service plan.
         :param storage_account_name: The name of the storage account. Should be unique across Azure.
         :param cdn_host: A custom CDN host name (optional)
+        :param comms_data_location: The data location for the Communication Services (optional if you don't need it)
         :param opts: The resource options
         """
 
         super().__init__("pkg:index:DjangoDeployment", name, None, opts)
 
         # child_opts = pulumi.ResourceOptions(parent=self)
 
@@ -340,14 +342,59 @@
             azure.web.WebAppHostNameBinding(
                 f"host-binding-{suffix}-{safe_host}",
                 resource_group_name=self._rg,
                 name=app.name,
                 host_name=host,
             )
 
+    def _add_webapp_comms(self, data_location: str, domains: list[str], suffix: str) -> azure.communication.CommunicationService:
+        email_service = azure.communication.EmailService(
+            f"comms-email-{suffix}",
+            resource_group_name=self._rg,
+            location="global",
+            data_location=data_location,
+        )
+
+        domain_resources = []
+        if domains:
+            # Add our own custom domains
+            for domain in domains:
+                safe_host = domain.replace(".", "-")
+                d = azure.communication.Domain(
+                    f"comms-email-domain-{suffix}-{safe_host}",
+                    resource_group_name=self._rg,
+                    location="global",
+                    domain_management=azure.communication.DomainManagement.CUSTOMER_MANAGED,
+                    domain_name=domain,
+                    email_service_name=email_service.name,
+                )
+                domain_resources.append(d.id.apply(lambda n: n))
+        else:
+            # Add an Azure managed domain
+            d = azure.communication.Domain(
+                f"comms-email-domain-{suffix}-azure",
+                resource_group_name=self._rg,
+                location="global",
+                domain_management=azure.communication.DomainManagement.AZURE_MANAGED,
+                domain_name="AzureManagedDomain",
+                email_service_name=email_service.name,
+            )
+            domain_resources.append(d.id.apply(lambda n: n))
+
+        # Create Communication Services and link the domains
+        comm_service = azure.communication.CommunicationService(
+            f"comms-{suffix}",
+            resource_group_name=self._rg,
+            location="global",
+            data_location=data_location,
+            linked_domains=domain_resources,
+        )
+
+        return comm_service
+
     def _get_storage_account_access_keys(
         self, storage_account: azure.storage.StorageAccount
     ) -> Sequence[azure.storage.outputs.StorageAccountKeyResponse]:
         """
         Helper function to get the access keys for a storage account.
 
         :param storage_account: The storage account
@@ -386,25 +433,29 @@
         name: str,
         db_name: str,
         repository_url: str,
         repository_branch: str,
         website_hosts: list[str],
         django_settings_module: str,
         environment_variables: dict[str, str] = {},
+        comms_data_location: Optional[str] = None,
+        comms_domains: Optional[list[str]] = [],
     ) -> azure.web.WebApp:
         """
         Create a Django website with it's own database and storage containers.
 
         :param name: The reference for the website, will be used to name subresources.
         :param db_name: The name of the database to create.
         :param repository_url: The URL of the Git repository.
         :param repository_branch: The Git branch to deploy.
         :param website_hosts: The list of custom host names for the website.
         :param django_settings_module: The Django settings module to load.
         :param environment_variables: A dictionary of environment variables to set.
+        :param comms_data_location: The data location for the Communication Services (optional if you don't need it).
+        :param comms_domains: The list of custom domains for the E-mail Communication Services (optional).
         """
 
         # Create a database
         db = azure.dbforpostgresql.Database(
             f"db-{name}",
             database_name=db_name,
             resource_group_name=self._rg,
@@ -425,14 +476,22 @@
             f"storage-container-{name}-static-{self._name}",
             resource_group_name=self._rg,
             account_name=self._storage_account.name,
             public_access=azure.storage.PublicAccess.BLOB,
             container_name=f"{name}-static",
         )
 
+        # Communication Services (optional)
+        if comms_data_location:
+            comms = self._add_webapp_comms(comms_data_location, comms_domains, f"{name}-{self._name}")
+            # Add the domains as environment variable
+            environment_variables["AZURE_COMMUNICATION_SERVICE"] = comms.name
+        else:
+            comms = None
+
         # Create a Django Secret Key (random)
         secret_key = pulumi_random.RandomString(f"django-secret-{name}-{self._name}", length=50)
 
         # Convert environment variables to NameValuePairArgs
         environment_variables = [
             azure.web.NameValuePairArgs(
                 name=key,
@@ -526,14 +585,32 @@
             f"ra-{name}-storage",
             principal_id=principal_id,
             principal_type=azure.authorization.PrincipalType.SERVICE_PRINCIPAL,
             role_definition_id=storage_role.id,
             scope=self._storage_account.id,
         )
 
+        # Grant the app to send e-mails
+        if comms:
+            comms_role = comms.id.apply(
+                lambda scope: azure.authorization.get_role_definition(
+                    # Contributor
+                    role_definition_id="b24988ac-6180-42a0-ab88-20f7382dd24c",
+                    scope=scope,
+                )
+            )
+
+            azure.authorization.RoleAssignment(
+                f"ra-{name}-comms",
+                principal_id=principal_id,
+                principal_type=azure.authorization.PrincipalType.SERVICE_PRINCIPAL,
+                role_definition_id=comms_role.id,
+                scope=comms.id,
+            )
+
         # Create a CORS rules for this website
         if website_hosts:
             origins = [f"https://{host}" for host in website_hosts]
         else:
             origins = ["*"]
 
         azure.storage.BlobServiceProperties(
```

### Comparing `pulumi-django-azure-1.0.6/src/pulumi_django_azure.egg-info/PKG-INFO` & `pulumi-django-azure-1.0.7/src/pulumi_django_azure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-django-azure
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simply deployment of Django on Azure with Pulumi
 Author-email: Maarten Ureel <maarten@youreal.eu>
 License: MIT License
         
         Copyright (c) 2023 YouReal BV
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,14 +41,15 @@
 
 This project aims to make a simple Django deployment on Azure easier.
 
 To have a proper and secure environment, we need these components:
 * Storage account for media and static files
 * CDN endpoint in front with a domain name of our choosing
 * PostgreSQL server
+* Azure Communication Services to send e-mails
 * Webapp with multiple custom host names and managed SSL for the website itself
 * Webapp running pgAdmin
 
 ## Installation
 This package is published on PyPi, so you can just add pulumi-django-azure to your requirements file.
 
 To use a specific branch in your project, add to pyproject.toml dependencies:
@@ -97,14 +98,16 @@
 django.add_django_website(
     name="web",
     db_name="mywebsite",
     repository_url="git@gitlab.com:project/website.git",
     repository_branch="main",
     website_hosts=["example.com", "www.example.com"],
     django_settings_module="mywebsite.settings.production",
+    comms_data_location="europe",
+    comms_domains=["mydomain.com"],
 )
 
 django.add_database_administrator(
     object_id="a1b2c3....",
     user_name="user@example.com",
     tenant_id="a1b2c3....",
 )
@@ -116,14 +119,15 @@
 2. Configure the PostgreSQL server (create and grant permissions to role for your websites)
 3. Retrieve the deployment SSH key and configure your remote GIT repository with it
 4. Configure your CDN host (add the CNAME record)
 5. Configure your custom website domains (add CNAME/A record and TXT validation records)
 6. Re-deploy with custom hosts
 7. Re-deploy once more to enable HTTPS on website domains
 8. Manually activate HTTPS on the CDN host
+9. Go to the e-mail communications service on Azure and configure DKIM, SPF,... for your custom domains.
 
 ## Custom domain name for CDN
 When deploying the first time, you will get a `cdn_cname` output. You need to create a CNAME to this domain before the deployment of the custom domain will succeed.
 
 You can safely deploy with the failing CustomDomain to get the CNAME, create the record and then deploy again.
 
 To enable HTTPS, you need to do this manually in the console. This is because of a limitation in the Azure API:
```

