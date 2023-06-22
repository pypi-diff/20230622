# Comparing `tmp/kegstandcli-0.3.8.tar.gz` & `tmp/kegstandcli-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegstandcli-0.3.8.tar", max compression
+gzip compressed data, was "kegstandcli-0.3.9.tar", max compression
```

## Comparing `kegstandcli-0.3.8.tar` & `kegstandcli-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1077 2023-04-23 18:42:25.686572 kegstandcli-0.3.8/LICENSE
--rw-r--r--   0        0        0     6581 2023-05-08 18:20:56.097880 kegstandcli-0.3.8/README.md
--rw-r--r--   0        0        0     1545 2023-06-20 23:44:55.511652 kegstandcli-0.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-03 20:22:59.696056 kegstandcli-0.3.8/src/kegstandcli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 20:23:08.893322 kegstandcli-0.3.8/src/kegstandcli/cli/__init__.py
--rw-r--r--   0        0        0    16270 2023-05-04 22:42:38.140953 kegstandcli-0.3.8/src/kegstandcli/cli/__main__.py
--rw-r--r--   0        0        0     3647 2023-06-20 23:46:48.735908 kegstandcli-0.3.8/src/kegstandcli/cli/build.py
--rw-r--r--   0        0        0     2516 2023-06-20 07:09:06.056577 kegstandcli-0.3.8/src/kegstandcli/cli/config.py
--rw-r--r--   0        0        0      154 2023-04-12 22:03:29.068379 kegstandcli-0.3.8/src/kegstandcli/cli/default_lambda.py.tmpl
--rw-r--r--   0        0        0     1972 2023-06-18 10:54:43.324903 kegstandcli-0.3.8/src/kegstandcli/cli/deploy.py
--rw-r--r--   0        0        0     1179 2023-04-25 19:33:46.541089 kegstandcli-0.3.8/src/kegstandcli/cli/new.py
--rw-r--r--   0        0        0      241 2023-06-20 23:46:53.763777 kegstandcli-0.3.8/src/kegstandcli/cli/rest_api_gateway_health_check.py.tmpl
--rw-r--r--   0        0        0     1302 2023-05-04 22:42:38.147183 kegstandcli-0.3.8/src/kegstandcli/cli/teardown.py
--rw-r--r--   0        0        0        0 2023-04-03 20:23:36.547617 kegstandcli-0.3.8/src/kegstandcli/infra/__init__.py
--rw-r--r--   0        0        0     3747 2023-06-20 23:47:10.853582 kegstandcli-0.3.8/src/kegstandcli/infra/app.py
--rw-r--r--   0        0        0      275 2023-04-27 20:31:57.718526 kegstandcli-0.3.8/src/kegstandcli/infra/cdk.json
--rw-r--r--   0        0        0        0 2023-04-03 20:23:50.899135 kegstandcli-0.3.8/src/kegstandcli/infra/stacks/__init__.py
--rw-r--r--   0        0        0     3989 2023-06-20 23:46:59.497383 kegstandcli-0.3.8/src/kegstandcli/infra/stacks/rest_api_backend.py
--rw-r--r--   0        0        0     7040 2023-06-20 23:47:03.474197 kegstandcli-0.3.8/src/kegstandcli/infra/stacks/rest_api_gateway.py
--rw-r--r--   0        0        0     1738 2023-06-20 23:47:15.485078 kegstandcli-0.3.8/src/kegstandcli/utils.py
--rw-r--r--   0        0        0     7899 1970-01-01 00:00:00.000000 kegstandcli-0.3.8/setup.py
--rw-r--r--   0        0        0     7959 1970-01-01 00:00:00.000000 kegstandcli-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-23 18:42:25.686572 kegstandcli-0.3.9/LICENSE
+-rw-r--r--   0        0        0     6623 2023-06-22 20:11:53.795514 kegstandcli-0.3.9/README.md
+-rw-r--r--   0        0        0     1545 2023-06-22 20:31:40.790172 kegstandcli-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 20:22:59.696056 kegstandcli-0.3.9/src/kegstandcli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:08.893322 kegstandcli-0.3.9/src/kegstandcli/cli/__init__.py
+-rw-r--r--   0        0        0    16270 2023-05-04 22:42:38.140953 kegstandcli-0.3.9/src/kegstandcli/cli/__main__.py
+-rw-r--r--   0        0        0     3647 2023-06-20 23:46:48.735908 kegstandcli-0.3.9/src/kegstandcli/cli/build.py
+-rw-r--r--   0        0        0     2516 2023-06-20 07:09:06.056577 kegstandcli-0.3.9/src/kegstandcli/cli/config.py
+-rw-r--r--   0        0        0      154 2023-04-12 22:03:29.068379 kegstandcli-0.3.9/src/kegstandcli/cli/default_lambda.py.tmpl
+-rw-r--r--   0        0        0     1972 2023-06-18 10:54:43.324903 kegstandcli-0.3.9/src/kegstandcli/cli/deploy.py
+-rw-r--r--   0        0        0     1179 2023-04-25 19:33:46.541089 kegstandcli-0.3.9/src/kegstandcli/cli/new.py
+-rw-r--r--   0        0        0      241 2023-06-20 23:46:53.763777 kegstandcli-0.3.9/src/kegstandcli/cli/rest_api_gateway_health_check.py.tmpl
+-rw-r--r--   0        0        0     1302 2023-05-04 22:42:38.147183 kegstandcli-0.3.9/src/kegstandcli/cli/teardown.py
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:36.547617 kegstandcli-0.3.9/src/kegstandcli/infra/__init__.py
+-rw-r--r--   0        0        0     4567 2023-06-22 20:11:43.375902 kegstandcli-0.3.9/src/kegstandcli/infra/app.py
+-rw-r--r--   0        0        0      275 2023-04-27 20:31:57.718526 kegstandcli-0.3.9/src/kegstandcli/infra/cdk.json
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:50.899135 kegstandcli-0.3.9/src/kegstandcli/infra/stacks/__init__.py
+-rw-r--r--   0        0        0     4181 2023-06-22 20:11:33.461355 kegstandcli-0.3.9/src/kegstandcli/infra/stacks/rest_api_backend.py
+-rw-r--r--   0        0        0     6285 2023-06-22 20:29:35.640639 kegstandcli-0.3.9/src/kegstandcli/infra/stacks/rest_api_gateway.py
+-rw-r--r--   0        0        0     1948 2023-06-22 20:11:47.720456 kegstandcli-0.3.9/src/kegstandcli/utils.py
+-rw-r--r--   0        0        0     7942 1970-01-01 00:00:00.000000 kegstandcli-0.3.9/setup.py
+-rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 kegstandcli-0.3.9/PKG-INFO
```

### Comparing `kegstandcli-0.3.8/LICENSE` & `kegstandcli-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.8/README.md` & `kegstandcli-0.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,29 +44,30 @@
 
 ```shell
 # Using the Kegstand CLI
 > pipx install kegstandcli
 > keg new my-service
 
 # Using Copier
-> copier gh:JensRoland/kegstand-project-template my-service
+> copier copy -d project_name=my-service gh:JensRoland/kegstand-project-template .
 ```
 
 Either method will create a new project folder called `my-service` containing:
 
 ```shell
 my-service
 ├── .gitignore                        # Standard .gitignore file
 ├── pyproject.toml                    # Project configuration
 └── src
     └── api
-        └── hello.py                  # Logic for /hello/
+        └── public
+            └── hello.py              # Logic for /hello/
 ```
 
-Kegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a single, empty `__init__.py` gatecrasher, but we can safely ignore that one.
+Kegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a few empty `__init__.py` gatecrashers, but we can safely ignore those.
 
 To install the dependencies for the new project:
 
 ```shell
 > cd my-service
 > poetry install
 ```
@@ -87,15 +88,15 @@
 
 Here are some notable changes, fixes and features that are planned for development:
 
 ## 0.4.0
 
 - [ ] More content on [kegstand.dev](https://kegstand.dev)
 - [x] Custom domain names
-- [ ] Support multiple repos using the same domain (and API Gateway)
+- [x] Support multiple repos using the same domain (and API Gateway)
 - [x] Simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
 
 ### Pre-1.0.0
 
 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.
 - [ ] Pagination helper
 - [ ] [Record a screencast](https://asciinema.org/) for the README
```

#### html2text {}

```diff
@@ -26,57 +26,57 @@
 docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended) - A
 well-poured [Belgian style brown ale](https://www.grimbergen.com/) ## Quick
 start To create a service with Kegstand, you'll need a Python project with a
 few dependencies and a folder structure following the Kegstand convention. You
 can create this in a few seconds, either with the Kegstand CLI or using
 [Copier](https://copier.readthedocs.io/en/stable/#installation). ```shell #
 Using the Kegstand CLI > pipx install kegstandcli > keg new my-service # Using
-Copier > copier gh:JensRoland/kegstand-project-template my-service ``` Either
-method will create a new project folder called `my-service` containing:
-```shell my-service âââ .gitignore # Standard .gitignore file âââ
-pyproject.toml # Project configuration âââ src âââ api âââ
-hello.py # Logic for /hello/ ``` Kegstand projects are minimal by design, so a
-fresh project folder contains just those 3 files. Well, apart from a single,
-empty `__init__.py` gatecrasher, but we can safely ignore that one. To install
-the dependencies for the new project: ```shell > cd my-service > poetry install
-``` Finally, to build and deploy the service to AWS: ```shell > poetry run keg
-deploy ``` You should now be able to access the API endpoint at `https:/
-/.execute-api..amazonaws.com/prod/hello`. ## Documentation For further examples
-and more advanced usage, see the [official documentation](https://github.com/
-JensRoland/kegstand/blob/main/docs/index.md). ## Roadmap Here are some notable
-changes, fixes and features that are planned for development: ## 0.4.0 - [ ]
-More content on [kegstand.dev](https://kegstand.dev) - [x] Custom domain names
-- [ ] Support multiple repos using the same domain (and API Gateway) - [x]
-Simplify the folder structure from `src/api/resources//.py` to `src/api/.py`
-### Pre-1.0.0 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS,
-DynamoDB, Cloudwatch CRON scheduled events, etc. - [ ] Pagination helper - [ ]
-[Record a screencast](https://asciinema.org/) for the README - [ ]
-Autogenerated docs using [MkDocs](https://www.mkdocs.org/) - [ ] GitHub Actions
-workflow for pushing docs to the website ### 1.0.0 - [ ] Intuitive and mostly
-automated API Versioning - [ ] Simple way to define/override core API/Lambda
-properties such as CPU/MEM, Python runtime version, warm pool (!), and
-concurrency - [ ] Deploy Lambda-only microservices with no API Gateway ###
-Future - [ ] Configurable log level - [ ] Add AWS tags in the Kegstand config
-and they will be applied to the generated resources - [ ] Easily add [AWS
-Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
-layers.html) - [ ] Add support for APIs using [FastAPI](https://
-fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default
-Kegstand API framework, and just provide deployment helpers for the API Gateway
-and Lambda - [ ] Improved output from deploy command; friendly post-deploy
-instructions for testing your API - [ ] Version bumper with [bump2version]
-(https://pypi.org/project/bump2version/) - [ ] Include more goodies from
-[Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/
-2.11.0/) - tracing, metrics, etc. - [ ] Add support for APIs using pure [Lambda
-Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/
+Copier > copier copy -d project_name=my-service gh:JensRoland/kegstand-project-
+template . ``` Either method will create a new project folder called `my-
+service` containing: ```shell my-service âââ .gitignore # Standard
+.gitignore file âââ pyproject.toml # Project configuration âââ src
+âââ api âââ public âââ hello.py # Logic for /hello/ ```
+Kegstand projects are minimal by design, so a fresh project folder contains
+just those 3 files. Well, apart from a few empty `__init__.py` gatecrashers,
+but we can safely ignore those. To install the dependencies for the new
+project: ```shell > cd my-service > poetry install ``` Finally, to build and
+deploy the service to AWS: ```shell > poetry run keg deploy ``` You should now
+be able to access the API endpoint at `https://.execute-api..amazonaws.com/
+prod/hello`. ## Documentation For further examples and more advanced usage, see
+the [official documentation](https://github.com/JensRoland/kegstand/blob/main/
+docs/index.md). ## Roadmap Here are some notable changes, fixes and features
+that are planned for development: ## 0.4.0 - [ ] More content on [kegstand.dev]
+(https://kegstand.dev) - [x] Custom domain names - [x] Support multiple repos
+using the same domain (and API Gateway) - [x] Simplify the folder structure
+from `src/api/resources//.py` to `src/api/.py` ### Pre-1.0.0 - [ ] Specify
+event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON
+scheduled events, etc. - [ ] Pagination helper - [ ] [Record a screencast]
+(https://asciinema.org/) for the README - [ ] Autogenerated docs using [MkDocs]
+(https://www.mkdocs.org/) - [ ] GitHub Actions workflow for pushing docs to the
+website ### 1.0.0 - [ ] Intuitive and mostly automated API Versioning - [ ]
+Simple way to define/override core API/Lambda properties such as CPU/MEM,
+Python runtime version, warm pool (!), and concurrency - [ ] Deploy Lambda-only
+microservices with no API Gateway ### Future - [ ] Configurable log level - [ ]
+Add AWS tags in the Kegstand config and they will be applied to the generated
+resources - [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/
+lambda/latest/dg/configuration-layers.html) - [ ] Add support for APIs using
+[FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/
 ) instead of the default Kegstand API framework, and just provide deployment
-helpers for the API Gateway and Lambda - [ ] Unit testing helpers (wrap moto
-and make it all a little more DRY and intuitive) - [ ] Secure endpoints which
-require re-authentication (and/or MFA) so a refreshed token isnât enough (to,
-say, delete your account or change your credit card info) - [ ] Live Lambda
-development a la SST - [ ] Build and deploy gRPC endpoints (or similar
-alternative) - [ ] Build and deploy GraphQL endpoints - [ ] Build and deploy
-stream processors? - [ ] Option to teardown before deploying: `keg deploy --
-force-redeploy` - [ ] Use env vars to populate values in kegstand.toml - [ ]
-Merge Kegstand and Beth into one tool - [ ] CDK Pipelines - [ ] Support HTTP
-method-specific files (e.g. `get.py`, `post.py`, etc.) - [ ] Upgrade Copier
-once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/
-1037) is released
+helpers for the API Gateway and Lambda - [ ] Improved output from deploy
+command; friendly post-deploy instructions for testing your API - [ ] Version
+bumper with [bump2version](https://pypi.org/project/bump2version/) - [ ]
+Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-
+lambda-powertools-python/2.11.0/) - tracing, metrics, etc. - [ ] Add support
+for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-
+powertools-python/2.11.0/) instead of the default Kegstand API framework, and
+just provide deployment helpers for the API Gateway and Lambda - [ ] Unit
+testing helpers (wrap moto and make it all a little more DRY and intuitive) -
+[ ] Secure endpoints which require re-authentication (and/or MFA) so a
+refreshed token isnât enough (to, say, delete your account or change your
+credit card info) - [ ] Live Lambda development a la SST - [ ] Build and deploy
+gRPC endpoints (or similar alternative) - [ ] Build and deploy GraphQL
+endpoints - [ ] Build and deploy stream processors? - [ ] Option to teardown
+before deploying: `keg deploy --force-redeploy` - [ ] Use env vars to populate
+values in kegstand.toml - [ ] Merge Kegstand and Beth into one tool - [ ] CDK
+Pipelines - [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`,
+etc.) - [ ] Upgrade Copier once the [template-deleting bugfix](https://
+github.com/copier-org/copier/pull/1037) is released
```

### Comparing `kegstandcli-0.3.8/pyproject.toml` & `kegstandcli-0.3.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kegstandcli"
-version = "0.3.8"
+version = "0.3.9"
 description = "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/kegstand"
 homepage = "https://kegstand.dev"
 readme = "README.md"
 packages = [
```

### Comparing `kegstandcli-0.3.8/src/kegstandcli/cli/__main__.py` & `kegstandcli-0.3.9/src/kegstandcli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.8/src/kegstandcli/cli/build.py` & `kegstandcli-0.3.9/src/kegstandcli/cli/build.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.8/src/kegstandcli/cli/config.py` & `kegstandcli-0.3.9/src/kegstandcli/cli/config.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.8/src/kegstandcli/cli/deploy.py` & `kegstandcli-0.3.9/src/kegstandcli/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.8/src/kegstandcli/cli/new.py` & `kegstandcli-0.3.9/src/kegstandcli/cli/new.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.8/src/kegstandcli/cli/teardown.py` & `kegstandcli-0.3.9/src/kegstandcli/cli/teardown.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.8/src/kegstandcli/infra/app.py` & `kegstandcli-0.3.9/src/kegstandcli/infra/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+import boto3
 import click
 import os
 import sys
 
 import aws_cdk as cdk
 from aws_cdk import aws_apigateway as apigw
 from aws_cdk import aws_cognito as cognito
@@ -67,21 +68,42 @@
     )
 
     modules["api_gateway"] = api_gateway_construct
 
 if "api" in config:
     click.echo("Creating stack for [api]...")
 
-    gateway = (
-        apigw.RestApi.from_rest_api_id(
-            parent_stack, "RestApiGatewayReference", config["api"]["api_gateway_id"]
+    if "api_gateway_id" in config["api"]:
+        rest_api_id = config["api"]["api_gateway_id"]
+        # TODO: Move this to utils.py
+        # Get the root resource ID from the API Gateway
+        apigw_client = boto3.client("apigateway", region_name=region)
+        response = apigw_client.get_resources(
+            restApiId=rest_api_id
         )
-        if "api_gateway_id" in config["api"]
-        else modules["api_gateway"].api if "api_gateway" in modules else None
-    )
+        root_resource_id = [
+            resource["id"]
+            for resource in response["items"]
+            if resource["path"] == "/"
+        ]
+        if len(root_resource_id) == 0:
+            raise Exception("Could not find root resource ID for API Gateway")
+        click.echo(f"Found API Gateway root resource ID: {root_resource_id[0]}")
+        root_resource_id = root_resource_id[0]
+
+        gateway = apigw.RestApi.from_rest_api_attributes(
+            parent_stack,
+            "RestApiGatewayReference",
+            rest_api_id=rest_api_id,
+            root_resource_id=root_resource_id,
+        )
+    else:
+        gateway = modules["api_gateway"].api if "api_gateway" in modules else None
+
+    
     user_pool = parent_stack.node.try_find_child("UserPool") if "api_gateway" in modules else (
         cognito.UserPool.from_user_pool_id(
             parent_stack, "UserPool", config["api"]["user_pool_id"]
         )
         if "user_pool_id" in config["api"]
         else None
     )
```

### Comparing `kegstandcli-0.3.8/src/kegstandcli/infra/stacks/rest_api_backend.py` & `kegstandcli-0.3.9/src/kegstandcli/infra/stacks/rest_api_backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,17 +74,19 @@
                     resource["name"],
                     default_integration=apigw.LambdaIntegration(self.lambda_function),
                     default_method_options=apigw.MethodOptions(
                         authorization_type=apigw.AuthorizationType.COGNITO,
                         authorizer=self.authorizer,  # Apply the authorizer
                     ),
                 )
+                resource_root.add_method("ANY", apigw.LambdaIntegration(self.lambda_function))
                 resource_root.add_proxy()
             else:
                 # Public (no auth required) endpoints
                 resource_root = rest_api_gw.root.add_resource(
                     resource["name"],
                     default_integration=apigw.LambdaIntegration(self.lambda_function)
                 )
+                resource_root.add_method("ANY", apigw.LambdaIntegration(self.lambda_function))
                 resource_root.add_proxy()
 
         self.deployment = apigw.Deployment(self, f"{id}-Deployment", api=rest_api_gw)
```

### Comparing `kegstandcli-0.3.8/src/kegstandcli/infra/stacks/rest_api_gateway.py` & `kegstandcli-0.3.9/src/kegstandcli/infra/stacks/rest_api_gateway.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,29 +126,12 @@
                 lambda_function_props=default_function_props,
                 api_gateway_props=api_gateway_props,
             )
 
         self.api = api_gateway_to_lambda.api_gateway
         self.health_check_function = api_gateway_to_lambda.lambda_function
 
-        self.authorizer = None
-        # if provision_with_authorizer:
-        #     click.echo("Creating Cognito authorizer for API Gateway...")
-        #     self.authorizer = apigw.CognitoUserPoolsAuthorizer(
-        #         self, f"{id}-Authorizer", cognito_user_pools=[user_pool]
-        #     )
-            # Add the authorizer to the API Gateway
-            # self.api.root.add_proxy(
-            #     default_method_options=apigw.MethodOptions(
-            #         authorization_type=apigw.AuthorizationType.COGNITO,
-            #         authorizer=self.authorizer,  # Apply the authorizer
-            #     ),
-            # )
-
         # For each resource, create API Gateway endpoints with the Lambda integration
         resource_root = self.api.root.add_resource("health")
-        # Health endpoint is always public (no auth required)
-        resource_root.add_proxy(
-            default_integration=apigw.LambdaIntegration(health_lambda_function)
-        )
+        resource_root.add_method("GET", apigw.LambdaIntegration(health_lambda_function))
 
         self.deployment = apigw.Deployment(self, f"{id}-Deployment", api=self.api)
```

### Comparing `kegstandcli-0.3.8/src/kegstandcli/utils.py` & `kegstandcli-0.3.9/src/kegstandcli/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 
+import click
+
 
 def find_resource_modules(api_src_dir: str) -> list:
     # Look through folder structure and create a list of resource modules found.
     # Expects a folder structure like this:
     #   api/
     #       [resource_name].py which exposes a resource object named `api`
     #   api/public/
@@ -14,14 +16,19 @@
         {"name": "api", "resources_are_public": False},
         {"name": "api/public", "resources_are_public": True},
     ]
 
     # Loop over folders in api_src_dir and list the resource modules
     for api_folder in api_folders:
         api_folder_full = os.path.join(api_src_dir, api_folder["name"])
+        if not os.path.isdir(api_folder_full):
+            click.echo(
+                f"API source folder {api_folder_full} does not exist, skipping..."
+            )
+            continue
         for file_descriptor in os.listdir(api_folder_full):
             # Ignore folders, only look at files
             if os.path.isdir(os.path.join(api_folder_full, file_descriptor)):
                 continue
             # Skip dotfiles and special files
             if (
                 file_descriptor.startswith(".")
```

### Comparing `kegstandcli-0.3.8/setup.py` & `kegstandcli-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
  'xxhash>=3.2.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['keg = kegstandcli.cli.__main__:kegstandcli']}
 
 setup_kwargs = {
     'name': 'kegstandcli',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
-    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://kegstand.dev/">\n    <img src="https://kegstand.dev/assets/kegstand-logotype.png" width="540px" alt="Kegstand logo" />\n  </a>\n</p>\n\n<h3 align="center">The Developer\'s Toolbelt For Accelerating <em>Mean Time To Party</em> on AWS</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a> and fueled by a non-zero amount of alcohol</p>\n<p align="center"><a href="https://kegstand.dev/demo">Watch a 3-minute demo</a></p><!-- markdown-link-check-disable-line -->\n\n<br />\n\n## 🥂💃🕺 Welcome to the Party! 🥂💃🕺\n\nKegstand is a free and open-source framework for creating Python APIs and services. It allows you to rapidly build and deploy services on AWS. We all have better things to do than `print(json.dumps(event))` all day long, and Kegstand is here to help you get to the party &mdash; _and into Prod_ &mdash; a lot faster.\n\n**It provides:**\n\n- A CLI tool for creating and deploying your services.\n- A decorator based API abstracting away the boilerplate of Lambda, API Gateway, Cognito, and more.\n- The full power of CDK to define and deploy arbitrary AWS resources with your services.\n\n> _"Experience a streamlined cloud development process, enhanced productivity, and hit that "party" button sooner with Kegstand!"_ > **&mdash; GPT-4, official spokesbot for the Kegstand team**\n\nLearn more on the [Kegstand website](https://kegstand.dev/).\n\n## Prerequisites\n\n- [Python 3.8+](https://www.python.org/downloads/)\n- [Poetry](https://python-poetry.org/docs/#installation) (recommended)\n- An [AWS account](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)\n- The [CDK CLI configured on the local machine and initialized on the AWS account](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)\n- The AWS CLI [configured with credentials](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)\n- [Copier](https://copier.readthedocs.io/en/stable/#installation) project scaffolding tool (recommended)\n- [npx](https://docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended)\n- A well-poured [Belgian style brown ale](https://www.grimbergen.com/)\n\n## Quick start\n\nTo create a service with Kegstand, you\'ll need a Python project with a few dependencies and a folder structure following the Kegstand convention.\n\nYou can create this in a few seconds, either with the Kegstand CLI or using [Copier](https://copier.readthedocs.io/en/stable/#installation).\n\n```shell\n# Using the Kegstand CLI\n> pipx install kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier gh:JensRoland/kegstand-project-template my-service\n```\n\nEither method will create a new project folder called `my-service` containing:\n\n```shell\nmy-service\n├── .gitignore                        # Standard .gitignore file\n├── pyproject.toml                    # Project configuration\n└── src\n    └── api\n        └── hello.py                  # Logic for /hello/\n```\n\nKegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a single, empty `__init__.py` gatecrasher, but we can safely ignore that one.\n\nTo install the dependencies for the new project:\n\n```shell\n> cd my-service\n> poetry install\n```\n\nFinally, to build and deploy the service to AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to access the API endpoint at `https://<api-id>.execute-api.<region>.amazonaws.com/prod/hello`.\n\n## Documentation\n\nFor further examples and more advanced usage, see the [official documentation](https://github.com/JensRoland/kegstand/blob/main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on [kegstand.dev](https://kegstand.dev)\n- [x] Custom domain names\n- [ ] Support multiple repos using the same domain (and API Gateway)\n- [x] Simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ] Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/override core API/Lambda properties such as CPU/MEM, Python runtime version, warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags in the Kegstand config and they will be applied to the generated resources\n- [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Improved output from deploy command; friendly post-deploy instructions for testing your API\n- [ ] Version bumper with [bump2version](https://pypi.org/project/bump2version/)\n- [ ] Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Unit testing helpers (wrap moto and make it all a little more DRY and intuitive)\n- [ ] Secure endpoints which require re-authentication (and/or MFA) so a refreshed token isn’t enough (to, say, delete your account or change your credit card info)\n- [ ] Live Lambda development a la SST\n- [ ] Build and deploy gRPC endpoints (or similar alternative)\n- [ ] Build and deploy GraphQL endpoints\n- [ ] Build and deploy stream processors?\n- [ ] Option to teardown before deploying: `keg deploy --force-redeploy`\n- [ ] Use env vars to populate values in kegstand.toml\n- [ ] Merge Kegstand and Beth into one tool\n- [ ] CDK Pipelines\n- [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`, etc.)\n- [ ] Upgrade Copier once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/1037) is released\n',
+    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://kegstand.dev/">\n    <img src="https://kegstand.dev/assets/kegstand-logotype.png" width="540px" alt="Kegstand logo" />\n  </a>\n</p>\n\n<h3 align="center">The Developer\'s Toolbelt For Accelerating <em>Mean Time To Party</em> on AWS</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a> and fueled by a non-zero amount of alcohol</p>\n<p align="center"><a href="https://kegstand.dev/demo">Watch a 3-minute demo</a></p><!-- markdown-link-check-disable-line -->\n\n<br />\n\n## 🥂💃🕺 Welcome to the Party! 🥂💃🕺\n\nKegstand is a free and open-source framework for creating Python APIs and services. It allows you to rapidly build and deploy services on AWS. We all have better things to do than `print(json.dumps(event))` all day long, and Kegstand is here to help you get to the party &mdash; _and into Prod_ &mdash; a lot faster.\n\n**It provides:**\n\n- A CLI tool for creating and deploying your services.\n- A decorator based API abstracting away the boilerplate of Lambda, API Gateway, Cognito, and more.\n- The full power of CDK to define and deploy arbitrary AWS resources with your services.\n\n> _"Experience a streamlined cloud development process, enhanced productivity, and hit that "party" button sooner with Kegstand!"_ > **&mdash; GPT-4, official spokesbot for the Kegstand team**\n\nLearn more on the [Kegstand website](https://kegstand.dev/).\n\n## Prerequisites\n\n- [Python 3.8+](https://www.python.org/downloads/)\n- [Poetry](https://python-poetry.org/docs/#installation) (recommended)\n- An [AWS account](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)\n- The [CDK CLI configured on the local machine and initialized on the AWS account](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)\n- The AWS CLI [configured with credentials](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)\n- [Copier](https://copier.readthedocs.io/en/stable/#installation) project scaffolding tool (recommended)\n- [npx](https://docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended)\n- A well-poured [Belgian style brown ale](https://www.grimbergen.com/)\n\n## Quick start\n\nTo create a service with Kegstand, you\'ll need a Python project with a few dependencies and a folder structure following the Kegstand convention.\n\nYou can create this in a few seconds, either with the Kegstand CLI or using [Copier](https://copier.readthedocs.io/en/stable/#installation).\n\n```shell\n# Using the Kegstand CLI\n> pipx install kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier copy -d project_name=my-service gh:JensRoland/kegstand-project-template .\n```\n\nEither method will create a new project folder called `my-service` containing:\n\n```shell\nmy-service\n├── .gitignore                        # Standard .gitignore file\n├── pyproject.toml                    # Project configuration\n└── src\n    └── api\n        └── public\n            └── hello.py              # Logic for /hello/\n```\n\nKegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a few empty `__init__.py` gatecrashers, but we can safely ignore those.\n\nTo install the dependencies for the new project:\n\n```shell\n> cd my-service\n> poetry install\n```\n\nFinally, to build and deploy the service to AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to access the API endpoint at `https://<api-id>.execute-api.<region>.amazonaws.com/prod/hello`.\n\n## Documentation\n\nFor further examples and more advanced usage, see the [official documentation](https://github.com/JensRoland/kegstand/blob/main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on [kegstand.dev](https://kegstand.dev)\n- [x] Custom domain names\n- [x] Support multiple repos using the same domain (and API Gateway)\n- [x] Simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ] Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/override core API/Lambda properties such as CPU/MEM, Python runtime version, warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags in the Kegstand config and they will be applied to the generated resources\n- [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Improved output from deploy command; friendly post-deploy instructions for testing your API\n- [ ] Version bumper with [bump2version](https://pypi.org/project/bump2version/)\n- [ ] Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Unit testing helpers (wrap moto and make it all a little more DRY and intuitive)\n- [ ] Secure endpoints which require re-authentication (and/or MFA) so a refreshed token isn’t enough (to, say, delete your account or change your credit card info)\n- [ ] Live Lambda development a la SST\n- [ ] Build and deploy gRPC endpoints (or similar alternative)\n- [ ] Build and deploy GraphQL endpoints\n- [ ] Build and deploy stream processors?\n- [ ] Option to teardown before deploying: `keg deploy --force-redeploy`\n- [ ] Use env vars to populate values in kegstand.toml\n- [ ] Merge Kegstand and Beth into one tool\n- [ ] CDK Pipelines\n- [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`, etc.)\n- [ ] Upgrade Copier once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/1037) is released\n',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kegstand.dev',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 'src'} packages = \ ['kegstandcli', 'kegstandcli.cli', 'kegstandcli.infra',
 'kegstandcli.infra.stacks'] package_data = \ {'': ['*']} install_requires = \
 ['aws-cdk-lib>=2.67.0,<3.0.0', 'aws-solutions-constructs-aws-apigateway-
 lambda>=2.39.0,<3.0.0', 'boto3>=1.17.113,<2.0.0', 'click>=8.0.3,<9.0.0',
 'constructs>=10.0.0,<11.0.0', 'copier>=6.2.0,<7.0.0', 'pyjwt>=2.1.0,<3.0.0',
 'tomlkit>=0.11.7,<0.12.0', 'xxhash>=3.2.0,<4.0.0'] entry_points = \
 {'console_scripts': ['keg = kegstandcli.cli.__main__:kegstandcli']}
-setup_kwargs = { 'name': 'kegstandcli', 'version': '0.3.8', 'description': "The
+setup_kwargs = { 'name': 'kegstandcli', 'version': '0.3.9', 'description': "The
 Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
 'long_description': '\n
                            \n \n_[Kegstand_logo]\n\n
 \n\n
 **** The Developer\'s Toolbelt For Accelerating Mean Time To Party on AWS ****
 \n
        Created by Jens_Roland and fueled by a non-zero amount of alcohol
@@ -40,64 +40,65 @@
 docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended)\n- A
 well-poured [Belgian style brown ale](https://www.grimbergen.com/)\n\n## Quick
 start\n\nTo create a service with Kegstand, you\'ll need a Python project with
 a few dependencies and a folder structure following the Kegstand
 convention.\n\nYou can create this in a few seconds, either with the Kegstand
 CLI or using [Copier](https://copier.readthedocs.io/en/stable/
 #installation).\n\n```shell\n# Using the Kegstand CLI\n> pipx install
-kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier gh:JensRoland/
-kegstand-project-template my-service\n```\n\nEither method will create a new
-project folder called `my-service` containing:\n\n```shell\nmy-
-service\nâââ .gitignore # Standard .gitignore file\nâââ
-pyproject.toml # Project configuration\nâââ src\n âââ api\n
-âââ hello.py # Logic for /hello/\n```\n\nKegstand projects are minimal by
-design, so a fresh project folder contains just those 3 files. Well, apart from
-a single, empty `__init__.py` gatecrasher, but we can safely ignore that
-one.\n\nTo install the dependencies for the new project:\n\n```shell\n> cd my-
-service\n> poetry install\n```\n\nFinally, to build and deploy the service to
-AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to
-access the API endpoint at `https://.execute-api..amazonaws.com/prod/
-hello`.\n\n## Documentation\n\nFor further examples and more advanced usage,
-see the [official documentation](https://github.com/JensRoland/kegstand/blob/
-main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and
-features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on
-[kegstand.dev](https://kegstand.dev)\n- [x] Custom domain names\n- [ ] Support
-multiple repos using the same domain (and API Gateway)\n- [x] Simplify the
-folder structure from `src/api/resources//.py` to `src/api/.py`\n\n### Pre-
-1.0.0\n\n- [ ] Specify event triggers for Lambda functions: S3, SNS, SQS,
-DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n-
-[ ] [Record a screencast](https://asciinema.org/) for the README\n- [ ]
-Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub
-Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ]
-Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/
-override core API/Lambda properties such as CPU/MEM, Python runtime version,
-warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no
-API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags
-in the Kegstand config and they will be applied to the generated resources\n-
-[ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/
-dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI]
-(https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of
-the default Kegstand API framework, and just provide deployment helpers for the
-API Gateway and Lambda\n- [ ] Improved output from deploy command; friendly
-post-deploy instructions for testing your API\n- [ ] Version bumper with
-[bump2version](https://pypi.org/project/bump2version/)\n- [ ] Include more
-goodies from [Lambda Powertools](https://awslabs.github.io/aws-lambda-
-powertools-python/2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs
-using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-
-python/2.11.0/) instead of the default Kegstand API framework, and just provide
-deployment helpers for the API Gateway and Lambda\n- [ ] Unit testing helpers
-(wrap moto and make it all a little more DRY and intuitive)\n- [ ] Secure
-endpoints which require re-authentication (and/or MFA) so a refreshed token
-isnât enough (to, say, delete your account or change your credit card
-info)\n- [ ] Live Lambda development a la SST\n- [ ] Build and deploy gRPC
-endpoints (or similar alternative)\n- [ ] Build and deploy GraphQL endpoints\n-
-[ ] Build and deploy stream processors?\n- [ ] Option to teardown before
-deploying: `keg deploy --force-redeploy`\n- [ ] Use env vars to populate values
-in kegstand.toml\n- [ ] Merge Kegstand and Beth into one tool\n- [ ] CDK
-Pipelines\n- [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`,
-etc.)\n- [ ] Upgrade Copier once the [template-deleting bugfix](https://
-github.com/copier-org/copier/pull/1037) is released\n', 'author': 'JensRoland',
-'author_email': 'mail@jensroland.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://kegstand.dev', 'package_dir':
-package_dir, 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'entry_points': entry_points,
-'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
+kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier copy -
+d project_name=my-service gh:JensRoland/kegstand-project-template
+.\n```\n\nEither method will create a new project folder called `my-service`
+containing:\n\n```shell\nmy-service\nâââ .gitignore # Standard .gitignore
+file\nâââ pyproject.toml # Project configuration\nâââ src\n
+âââ api\n âââ public\n âââ hello.py # Logic for /hello/
+\n```\n\nKegstand projects are minimal by design, so a fresh project folder
+contains just those 3 files. Well, apart from a few empty `__init__.py`
+gatecrashers, but we can safely ignore those.\n\nTo install the dependencies
+for the new project:\n\n```shell\n> cd my-service\n> poetry
+install\n```\n\nFinally, to build and deploy the service to AWS:\n\n```shell\n>
+poetry run keg deploy\n```\n\nYou should now be able to access the API endpoint
+at `https://.execute-api..amazonaws.com/prod/hello`.\n\n## Documentation\n\nFor
+further examples and more advanced usage, see the [official documentation]
+(https://github.com/JensRoland/kegstand/blob/main/docs/index.md).\n\n##
+Roadmap\n\nHere are some notable changes, fixes and features that are planned
+for development:\n\n## 0.4.0\n\n- [ ] More content on [kegstand.dev](https://
+kegstand.dev)\n- [x] Custom domain names\n- [x] Support multiple repos using
+the same domain (and API Gateway)\n- [x] Simplify the folder structure from
+`src/api/resources//.py` to `src/api/.py`\n\n### Pre-1.0.0\n\n- [ ] Specify
+event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON
+scheduled events, etc.\n- [ ] Pagination helper\n- [ ] [Record a screencast]
+(https://asciinema.org/) for the README\n- [ ] Autogenerated docs using
+[MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub Actions workflow for pushing
+docs to the website\n\n### 1.0.0\n\n- [ ] Intuitive and mostly automated API
+Versioning\n- [ ] Simple way to define/override core API/Lambda properties such
+as CPU/MEM, Python runtime version, warm pool (!), and concurrency\n- [ ]
+Deploy Lambda-only microservices with no API Gateway\n\n### Future\n\n- [ ]
+Configurable log level\n- [ ] Add AWS tags in the Kegstand config and they will
+be applied to the generated resources\n- [ ] Easily add [AWS Lambda Layers]
+(https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)\n- [ ]
+Add support for APIs using [FastAPI](https://fastapi.tiangolo.com/) with
+[Mangum](https://mangum.io/) instead of the default Kegstand API framework, and
+just provide deployment helpers for the API Gateway and Lambda\n- [ ] Improved
+output from deploy command; friendly post-deploy instructions for testing your
+API\n- [ ] Version bumper with [bump2version](https://pypi.org/project/
+bump2version/)\n- [ ] Include more goodies from [Lambda Powertools](https://
+awslabs.github.io/aws-lambda-powertools-python/2.11.0/) - tracing, metrics,
+etc.\n- [ ] Add support for APIs using pure [Lambda Powertools](https://
+awslabs.github.io/aws-lambda-powertools-python/2.11.0/) instead of the default
+Kegstand API framework, and just provide deployment helpers for the API Gateway
+and Lambda\n- [ ] Unit testing helpers (wrap moto and make it all a little more
+DRY and intuitive)\n- [ ] Secure endpoints which require re-authentication
+(and/or MFA) so a refreshed token isnât enough (to, say, delete your account
+or change your credit card info)\n- [ ] Live Lambda development a la SST\n- [ ]
+Build and deploy gRPC endpoints (or similar alternative)\n- [ ] Build and
+deploy GraphQL endpoints\n- [ ] Build and deploy stream processors?\n- [ ]
+Option to teardown before deploying: `keg deploy --force-redeploy`\n- [ ] Use
+env vars to populate values in kegstand.toml\n- [ ] Merge Kegstand and Beth
+into one tool\n- [ ] CDK Pipelines\n- [ ] Support HTTP method-specific files
+(e.g. `get.py`, `post.py`, etc.)\n- [ ] Upgrade Copier once the [template-
+deleting bugfix](https://github.com/copier-org/copier/pull/1037) is
+released\n', 'author': 'JensRoland', 'author_email': 'mail@jensroland.com',
+'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://
+kegstand.dev', 'package_dir': package_dir, 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'entry_points': entry_points, 'python_requires': '>=3.9,<4.0', } setup
+(**setup_kwargs)
```

### Comparing `kegstandcli-0.3.8/PKG-INFO` & `kegstandcli-0.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegstandcli
-Version: 0.3.8
+Version: 0.3.9
 Summary: The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS
 Home-page: https://kegstand.dev
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -77,29 +77,30 @@
 
 ```shell
 # Using the Kegstand CLI
 > pipx install kegstandcli
 > keg new my-service
 
 # Using Copier
-> copier gh:JensRoland/kegstand-project-template my-service
+> copier copy -d project_name=my-service gh:JensRoland/kegstand-project-template .
 ```
 
 Either method will create a new project folder called `my-service` containing:
 
 ```shell
 my-service
 ├── .gitignore                        # Standard .gitignore file
 ├── pyproject.toml                    # Project configuration
 └── src
     └── api
-        └── hello.py                  # Logic for /hello/
+        └── public
+            └── hello.py              # Logic for /hello/
 ```
 
-Kegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a single, empty `__init__.py` gatecrasher, but we can safely ignore that one.
+Kegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a few empty `__init__.py` gatecrashers, but we can safely ignore those.
 
 To install the dependencies for the new project:
 
 ```shell
 > cd my-service
 > poetry install
 ```
@@ -120,15 +121,15 @@
 
 Here are some notable changes, fixes and features that are planned for development:
 
 ## 0.4.0
 
 - [ ] More content on [kegstand.dev](https://kegstand.dev)
 - [x] Custom domain names
-- [ ] Support multiple repos using the same domain (and API Gateway)
+- [x] Support multiple repos using the same domain (and API Gateway)
 - [x] Simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
 
 ### Pre-1.0.0
 
 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.
 - [ ] Pagination helper
 - [ ] [Record a screencast](https://asciinema.org/) for the README
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kegstandcli Version: 0.3.8 Summary: The Developer's
+Metadata-Version: 2.1 Name: kegstandcli Version: 0.3.9 Summary: The Developer's
 Toolbelt For Accelerating Mean-Time-To-Party on AWS Home-page: https://
 kegstand.dev License: MIT Author: JensRoland Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -45,57 +45,57 @@
 docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended) - A
 well-poured [Belgian style brown ale](https://www.grimbergen.com/) ## Quick
 start To create a service with Kegstand, you'll need a Python project with a
 few dependencies and a folder structure following the Kegstand convention. You
 can create this in a few seconds, either with the Kegstand CLI or using
 [Copier](https://copier.readthedocs.io/en/stable/#installation). ```shell #
 Using the Kegstand CLI > pipx install kegstandcli > keg new my-service # Using
-Copier > copier gh:JensRoland/kegstand-project-template my-service ``` Either
-method will create a new project folder called `my-service` containing:
-```shell my-service âââ .gitignore # Standard .gitignore file âââ
-pyproject.toml # Project configuration âââ src âââ api âââ
-hello.py # Logic for /hello/ ``` Kegstand projects are minimal by design, so a
-fresh project folder contains just those 3 files. Well, apart from a single,
-empty `__init__.py` gatecrasher, but we can safely ignore that one. To install
-the dependencies for the new project: ```shell > cd my-service > poetry install
-``` Finally, to build and deploy the service to AWS: ```shell > poetry run keg
-deploy ``` You should now be able to access the API endpoint at `https:/
-/.execute-api..amazonaws.com/prod/hello`. ## Documentation For further examples
-and more advanced usage, see the [official documentation](https://github.com/
-JensRoland/kegstand/blob/main/docs/index.md). ## Roadmap Here are some notable
-changes, fixes and features that are planned for development: ## 0.4.0 - [ ]
-More content on [kegstand.dev](https://kegstand.dev) - [x] Custom domain names
-- [ ] Support multiple repos using the same domain (and API Gateway) - [x]
-Simplify the folder structure from `src/api/resources//.py` to `src/api/.py`
-### Pre-1.0.0 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS,
-DynamoDB, Cloudwatch CRON scheduled events, etc. - [ ] Pagination helper - [ ]
-[Record a screencast](https://asciinema.org/) for the README - [ ]
-Autogenerated docs using [MkDocs](https://www.mkdocs.org/) - [ ] GitHub Actions
-workflow for pushing docs to the website ### 1.0.0 - [ ] Intuitive and mostly
-automated API Versioning - [ ] Simple way to define/override core API/Lambda
-properties such as CPU/MEM, Python runtime version, warm pool (!), and
-concurrency - [ ] Deploy Lambda-only microservices with no API Gateway ###
-Future - [ ] Configurable log level - [ ] Add AWS tags in the Kegstand config
-and they will be applied to the generated resources - [ ] Easily add [AWS
-Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
-layers.html) - [ ] Add support for APIs using [FastAPI](https://
-fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default
-Kegstand API framework, and just provide deployment helpers for the API Gateway
-and Lambda - [ ] Improved output from deploy command; friendly post-deploy
-instructions for testing your API - [ ] Version bumper with [bump2version]
-(https://pypi.org/project/bump2version/) - [ ] Include more goodies from
-[Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/
-2.11.0/) - tracing, metrics, etc. - [ ] Add support for APIs using pure [Lambda
-Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/
+Copier > copier copy -d project_name=my-service gh:JensRoland/kegstand-project-
+template . ``` Either method will create a new project folder called `my-
+service` containing: ```shell my-service âââ .gitignore # Standard
+.gitignore file âââ pyproject.toml # Project configuration âââ src
+âââ api âââ public âââ hello.py # Logic for /hello/ ```
+Kegstand projects are minimal by design, so a fresh project folder contains
+just those 3 files. Well, apart from a few empty `__init__.py` gatecrashers,
+but we can safely ignore those. To install the dependencies for the new
+project: ```shell > cd my-service > poetry install ``` Finally, to build and
+deploy the service to AWS: ```shell > poetry run keg deploy ``` You should now
+be able to access the API endpoint at `https://.execute-api..amazonaws.com/
+prod/hello`. ## Documentation For further examples and more advanced usage, see
+the [official documentation](https://github.com/JensRoland/kegstand/blob/main/
+docs/index.md). ## Roadmap Here are some notable changes, fixes and features
+that are planned for development: ## 0.4.0 - [ ] More content on [kegstand.dev]
+(https://kegstand.dev) - [x] Custom domain names - [x] Support multiple repos
+using the same domain (and API Gateway) - [x] Simplify the folder structure
+from `src/api/resources//.py` to `src/api/.py` ### Pre-1.0.0 - [ ] Specify
+event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON
+scheduled events, etc. - [ ] Pagination helper - [ ] [Record a screencast]
+(https://asciinema.org/) for the README - [ ] Autogenerated docs using [MkDocs]
+(https://www.mkdocs.org/) - [ ] GitHub Actions workflow for pushing docs to the
+website ### 1.0.0 - [ ] Intuitive and mostly automated API Versioning - [ ]
+Simple way to define/override core API/Lambda properties such as CPU/MEM,
+Python runtime version, warm pool (!), and concurrency - [ ] Deploy Lambda-only
+microservices with no API Gateway ### Future - [ ] Configurable log level - [ ]
+Add AWS tags in the Kegstand config and they will be applied to the generated
+resources - [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/
+lambda/latest/dg/configuration-layers.html) - [ ] Add support for APIs using
+[FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/
 ) instead of the default Kegstand API framework, and just provide deployment
-helpers for the API Gateway and Lambda - [ ] Unit testing helpers (wrap moto
-and make it all a little more DRY and intuitive) - [ ] Secure endpoints which
-require re-authentication (and/or MFA) so a refreshed token isnât enough (to,
-say, delete your account or change your credit card info) - [ ] Live Lambda
-development a la SST - [ ] Build and deploy gRPC endpoints (or similar
-alternative) - [ ] Build and deploy GraphQL endpoints - [ ] Build and deploy
-stream processors? - [ ] Option to teardown before deploying: `keg deploy --
-force-redeploy` - [ ] Use env vars to populate values in kegstand.toml - [ ]
-Merge Kegstand and Beth into one tool - [ ] CDK Pipelines - [ ] Support HTTP
-method-specific files (e.g. `get.py`, `post.py`, etc.) - [ ] Upgrade Copier
-once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/
-1037) is released
+helpers for the API Gateway and Lambda - [ ] Improved output from deploy
+command; friendly post-deploy instructions for testing your API - [ ] Version
+bumper with [bump2version](https://pypi.org/project/bump2version/) - [ ]
+Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-
+lambda-powertools-python/2.11.0/) - tracing, metrics, etc. - [ ] Add support
+for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-
+powertools-python/2.11.0/) instead of the default Kegstand API framework, and
+just provide deployment helpers for the API Gateway and Lambda - [ ] Unit
+testing helpers (wrap moto and make it all a little more DRY and intuitive) -
+[ ] Secure endpoints which require re-authentication (and/or MFA) so a
+refreshed token isnât enough (to, say, delete your account or change your
+credit card info) - [ ] Live Lambda development a la SST - [ ] Build and deploy
+gRPC endpoints (or similar alternative) - [ ] Build and deploy GraphQL
+endpoints - [ ] Build and deploy stream processors? - [ ] Option to teardown
+before deploying: `keg deploy --force-redeploy` - [ ] Use env vars to populate
+values in kegstand.toml - [ ] Merge Kegstand and Beth into one tool - [ ] CDK
+Pipelines - [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`,
+etc.) - [ ] Upgrade Copier once the [template-deleting bugfix](https://
+github.com/copier-org/copier/pull/1037) is released
```

