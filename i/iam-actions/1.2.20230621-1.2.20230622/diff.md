# Comparing `tmp/iam_actions-1.2.20230621.tar.gz` & `tmp/iam_actions-1.2.20230622.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230621.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230622.tar", max compression
```

## Comparing `iam_actions-1.2.20230621.tar` & `iam_actions-1.2.20230622.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/README.md
--rw-r--r--   0        0        0      228 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/__init__.py
--rw-r--r--   0        0        0  4337071 2023-06-21 02:33:30.119694 iam_actions-1.2.20230621/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/services.py
--rw-r--r--   0        0        0   557686 2023-06-21 02:33:30.119694 iam_actions-1.2.20230621/iam_actions/policies.json
--rw-r--r--   0        0        0   196535 2023-06-21 02:33:30.119694 iam_actions-1.2.20230621/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   540907 2023-06-21 02:33:30.119694 iam_actions-1.2.20230621/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-21 02:33:31.071767 iam_actions-1.2.20230621/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230621/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230621/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/README.md
+-rw-r--r--   0        0        0      228 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4339454 2023-06-22 02:38:18.882778 iam_actions-1.2.20230622/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   557867 2023-06-22 02:38:18.882778 iam_actions-1.2.20230622/iam_actions/policies.json
+-rw-r--r--   0        0        0   196684 2023-06-22 02:38:18.882778 iam_actions-1.2.20230622/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   541083 2023-06-22 02:38:18.882778 iam_actions-1.2.20230622/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-22 02:38:19.914865 iam_actions-1.2.20230622/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230622/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230622/PKG-INFO
```

### Comparing `iam_actions-1.2.20230621/LICENSE` & `iam_actions-1.2.20230622/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230621/README.md` & `iam_actions-1.2.20230622/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230621/iam_actions/actions.json` & `iam_actions-1.2.20230622/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998234811589646%*

 * *Differences: {"'auditmanager'": "{'GetEvidenceFileUploadUrl': {'access_level': 'Read', 'description': 'Grants "*

 * *                   'permission to get a presigned Amazon S3 URL that can be used to upload a file '*

 * *                   "as manual evidence'}}",*

 * * "'ec2'": "{'CreateTags': {'resources': {insert: [(20, 'instance-connect-endpoint')]}}, "*

 * *          "'DeleteTags': {'resources': {insert: [(20, 'instance-connect-endpoint')]}}, "*

 * *          "'CreateInstanceConnectEndpoint': OrderedDict([('access_level', 'Write'), ('acti […]*

```diff
@@ -9044,18 +9044,18 @@
             "description": "Grants permission to get all the evidence from an evidence folder in AWS Audit Manager",
             "orphan": false,
             "resources": [
                 "assessmentControlSet"
             ]
         },
         "GetEvidenceFileUploadUrl": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetEvidenceFileUploadUrl",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get a presigned Amazon S3 URL that can be used to upload a file as manual evidence",
             "orphan": false,
             "resources": []
         },
         "GetEvidenceFolder": {
             "access_level": "Read",
             "action": "GetEvidenceFolder",
             "condition_keys": [],
@@ -44004,14 +44004,36 @@
             "orphan": false,
             "resources": [
                 "image",
                 "instance",
                 "snapshot"
             ]
         },
+        "CreateInstanceConnectEndpoint": {
+            "access_level": "Write",
+            "action": "CreateInstanceConnectEndpoint",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AvailabilityZone",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to create an EC2 Instance Connect Endpoint that allows you to connect to an instance without a public IPv4 address",
+            "orphan": false,
+            "resources": [
+                "instance-connect-endpoint",
+                "security-group",
+                "subnet"
+            ]
+        },
         "CreateInstanceEventWindow": {
             "access_level": "Write",
             "action": "CreateInstanceEventWindow",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
                 "ec2:Region"
@@ -44821,14 +44843,15 @@
                 "fleet",
                 "fpga-image",
                 "host-reservation",
                 "image",
                 "import-image-task",
                 "import-snapshot-task",
                 "instance",
+                "instance-connect-endpoint",
                 "instance-event-window",
                 "internet-gateway",
                 "ipam",
                 "ipam-pool",
                 "ipam-resource-discovery",
                 "ipam-resource-discovery-association",
                 "ipam-scope",
@@ -45588,14 +45611,29 @@
             ],
             "description": "Grants permission to delete an Amazon FPGA Image (AFI)",
             "orphan": false,
             "resources": [
                 "fpga-image"
             ]
         },
+        "DeleteInstanceConnectEndpoint": {
+            "access_level": "Write",
+            "action": "DeleteInstanceConnectEndpoint",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID"
+            ],
+            "description": "Grants permission to delete an EC2 Instance Connect Endpoint",
+            "orphan": false,
+            "resources": [
+                "instance-connect-endpoint"
+            ]
+        },
         "DeleteInstanceEventWindow": {
             "access_level": "Write",
             "action": "DeleteInstanceEventWindow",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}"
@@ -46135,14 +46173,15 @@
                 "fleet",
                 "fpga-image",
                 "host-reservation",
                 "image",
                 "import-image-task",
                 "import-snapshot-task",
                 "instance",
+                "instance-connect-endpoint",
                 "instance-event-window",
                 "internet-gateway",
                 "ipam",
                 "ipam-pool",
                 "ipam-resource-discovery",
                 "ipam-resource-discovery-association",
                 "ipam-scope",
@@ -47263,14 +47302,24 @@
             ],
             "description": "Grants permission to describe the attributes of an instance",
             "orphan": false,
             "resources": [
                 "instance"
             ]
         },
+        "DescribeInstanceConnectEndpoints": {
+            "access_level": "List",
+            "action": "DescribeInstanceConnectEndpoints",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe EC2 Instance Connect Endpoints",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeInstanceCreditSpecifications": {
             "access_level": "List",
             "action": "DescribeInstanceCreditSpecifications",
             "condition_keys": [
                 "ec2:Region"
             ],
             "description": "Grants permission to describe the credit option for CPU usage of one or more burstable performance instances",
@@ -143553,183 +143602,199 @@
         }
     },
     "support": {
         "AddAttachmentsToSet": {
             "access_level": "Write",
             "action": "AddAttachmentsToSet",
             "condition_keys": [],
-            "description": "Adds one or more attachments to an AWS Support case.",
+            "description": "Grants permission to add one or more attachments to an AWS Support case",
             "orphan": false,
             "resources": []
         },
         "AddCommunicationToCase": {
             "access_level": "Write",
             "action": "AddCommunicationToCase",
             "condition_keys": [],
-            "description": "Adds a customer communication to an AWS Support case.",
+            "description": "Grants permission to add a customer communication to an AWS Support case",
             "orphan": false,
             "resources": []
         },
         "CreateCase": {
             "access_level": "Write",
             "action": "CreateCase",
             "condition_keys": [],
-            "description": "Creates a new AWS Support case.",
+            "description": "Grants permission to creates a new AWS Support case",
             "orphan": false,
             "resources": []
         },
         "DescribeAttachment": {
             "access_level": "Read",
             "action": "DescribeAttachment",
             "condition_keys": [],
-            "description": "Returns the description for an attachment.",
+            "description": "Grants permission to describe attachment detail",
             "orphan": false,
             "resources": []
         },
         "DescribeCaseAttributes": {
             "access_level": "Read",
             "action": "DescribeCaseAttributes",
             "condition_keys": [],
-            "description": "This is an internally managed function which allows secondary services to read AWS Support case attributes.",
+            "description": "Grants permission to allow secondary services to read AWS Support case attributes.This is an internally managed function",
             "orphan": false,
             "resources": []
         },
         "DescribeCases": {
             "access_level": "Read",
             "action": "DescribeCases",
             "condition_keys": [],
-            "description": "Returns a list of AWS Support cases that matches the given inputs.",
+            "description": "Grants permission to list AWS Support cases that matches the given inputs",
             "orphan": false,
             "resources": []
         },
         "DescribeCommunications": {
             "access_level": "Read",
             "action": "DescribeCommunications",
             "condition_keys": [],
-            "description": "Returns the communications and attachments for one or more AWS Support cases.",
+            "description": "Grants permission to list the communications and attachments for one or more AWS Support cases",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeCreateCaseOptions": {
+            "access_level": "Read",
+            "action": "DescribeCreateCaseOptions",
+            "condition_keys": [],
+            "description": "Grants permission to describes the available options for creating a support case",
             "orphan": false,
             "resources": []
         },
         "DescribeIssueTypes": {
             "access_level": "Read",
             "action": "DescribeIssueTypes",
             "condition_keys": [],
-            "description": "Returns issue types for AWS Support cases.",
+            "description": "Grants permission to return issue types for AWS Support cases",
             "orphan": false,
             "resources": []
         },
         "DescribeServices": {
             "access_level": "Read",
             "action": "DescribeServices",
             "condition_keys": [],
-            "description": "Returns the current list of AWS services and categories that applies to each service.",
+            "description": "Grants permission to list AWS services and categories that applies to each service",
             "orphan": false,
             "resources": []
         },
         "DescribeSeverityLevels": {
             "access_level": "Read",
             "action": "DescribeSeverityLevels",
             "condition_keys": [],
-            "description": "Returns the list of severity levels that can be assigned to an AWS Support case.",
+            "description": "Grants permission to list severity levels that can be assigned to an AWS Support case",
             "orphan": false,
             "resources": []
         },
         "DescribeSupportLevel": {
             "access_level": "Read",
             "action": "DescribeSupportLevel",
             "condition_keys": [],
-            "description": "Returns the support level for an AWS Account identifier.",
+            "description": "Grants permission to return the support level for an AWS Account identifier",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeSupportedLanguages": {
+            "access_level": "Read",
+            "action": "DescribeSupportedLanguages",
+            "condition_keys": [],
+            "description": "Grants permission to describes the available support languages for a given category code, service code and issue type",
             "orphan": false,
             "resources": []
         },
         "DescribeTrustedAdvisorCheckRefreshStatuses": {
             "access_level": "Read",
             "action": "DescribeTrustedAdvisorCheckRefreshStatuses",
             "condition_keys": [],
-            "description": "Returns the status of a Trusted Advisor refresh check based on a list of check identifiers.",
+            "description": "Grants permission to get the status of a Trusted Advisor refresh check based on a list of check identifiers",
             "orphan": false,
             "resources": []
         },
         "DescribeTrustedAdvisorCheckResult": {
             "access_level": "Read",
             "action": "DescribeTrustedAdvisorCheckResult",
             "condition_keys": [],
-            "description": "Returns the results of the Trusted Advisor check that has the specified check identifier.",
+            "description": "Grants permission to get the results of the Trusted Advisor check that has the specified check identifier",
             "orphan": false,
             "resources": []
         },
         "DescribeTrustedAdvisorCheckSummaries": {
             "access_level": "Read",
             "action": "DescribeTrustedAdvisorCheckSummaries",
             "condition_keys": [],
-            "description": "Returns the summaries of the results of the Trusted Advisor checks that have the specified check identifiers.",
+            "description": "Grants permission to get the summaries of the results of the Trusted Advisor checks that have the specified check identifiers",
             "orphan": false,
             "resources": []
         },
         "DescribeTrustedAdvisorChecks": {
             "access_level": "Read",
             "action": "DescribeTrustedAdvisorChecks",
             "condition_keys": [],
-            "description": "Returns a list of all available Trusted Advisor checks, including name, identifier, category and description.",
+            "description": "Grants permission to get a list of all available Trusted Advisor checks, including name, identifier, category and description",
             "orphan": false,
             "resources": []
         },
         "InitiateCallForCase": {
             "access_level": "Write",
             "action": "InitiateCallForCase",
             "condition_keys": [],
-            "description": "This is an internally managed function to initiate a call on AWS Support Center.",
+            "description": "Grants permission to initiate a call on AWS Support Center. This is an internally managed function",
             "orphan": false,
             "resources": []
         },
         "InitiateChatForCase": {
             "access_level": "Write",
             "action": "InitiateChatForCase",
             "condition_keys": [],
-            "description": "This is an internally managed function to initiate a chat on AWS Support Center.",
+            "description": "Grants permission to initiate a chat on AWS Support Center.This is an internally managed function",
             "orphan": false,
             "resources": []
         },
         "PutCaseAttributes": {
             "access_level": "Write",
             "action": "PutCaseAttributes",
             "condition_keys": [],
-            "description": "This is an internally managed function which allows secondary services to attach attributes to AWS Support cases.",
+            "description": "Grants permission to allow secondary services to attach attributes to AWS Support cases. This is an internally managed function",
             "orphan": false,
             "resources": []
         },
         "RateCaseCommunication": {
             "access_level": "Write",
             "action": "RateCaseCommunication",
             "condition_keys": [],
-            "description": "Rate an AWS Support case communication.",
+            "description": "Grants permission to rate an AWS Support case communication",
             "orphan": false,
             "resources": []
         },
         "RefreshTrustedAdvisorCheck": {
             "access_level": "Write",
             "action": "RefreshTrustedAdvisorCheck",
             "condition_keys": [],
-            "description": "Requests a refresh of the Trusted Advisor check that has the specified check identifier.",
+            "description": "Grants permission to requests a refresh of the Trusted Advisor check that has the specified check identifier",
             "orphan": false,
             "resources": []
         },
         "ResolveCase": {
             "access_level": "Write",
             "action": "ResolveCase",
             "condition_keys": [],
-            "description": "Resolves an AWS Support case.",
+            "description": "Grants permission to resolve an AWS Support case",
             "orphan": false,
             "resources": []
         },
         "SearchForCases": {
             "access_level": "Read",
             "action": "SearchForCases",
             "condition_keys": [],
-            "description": "Returns a list of AWS Support cases that matches the given inputs.",
+            "description": "Grants permission to return a list of AWS Support cases that matches the given inputs",
             "orphan": false,
             "resources": []
         }
     },
     "supportapp": {
         "CreateSlackChannelConfiguration": {
             "access_level": "Write",
```

### Comparing `iam_actions-1.2.20230621/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230622/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230621/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230622/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230621/iam_actions/generate/generate.py` & `iam_actions-1.2.20230622/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230621/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230622/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230621/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230622/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230621/iam_actions/generate/services.py` & `iam_actions-1.2.20230622/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230621/iam_actions/policies.json` & `iam_actions-1.2.20230622/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999981135358944%*

 * *Differences: {"'serviceMap'": "{'AWS Support': {'Actions': {insert: [(7, 'DescribeCreateCaseOptions'), (12, "*

 * *                 "'DescribeSupportedLanguages')]}}, 'Amazon EC2': {'Actions': {insert: [(72, "*

 * *                 "'CreateInstanceConnectEndpoint'), (151, 'DeleteInstanceConnectEndpoint'), (268, "*

 * *                 "'DescribeInstanceConnectEndpoints')]}}}"}*

```diff
@@ -8652,18 +8652,20 @@
                 "AddAttachmentsToSet",
                 "AddCommunicationToCase",
                 "CreateCase",
                 "DescribeAttachment",
                 "DescribeCaseAttributes",
                 "DescribeCases",
                 "DescribeCommunications",
+                "DescribeCreateCaseOptions",
                 "DescribeIssueTypes",
                 "DescribeServices",
                 "DescribeSeverityLevels",
                 "DescribeSupportLevel",
+                "DescribeSupportedLanguages",
                 "DescribeTrustedAdvisorCheckRefreshStatuses",
                 "DescribeTrustedAdvisorCheckResult",
                 "DescribeTrustedAdvisorCheckSummaries",
                 "DescribeTrustedAdvisorChecks",
                 "InitiateCallForCase",
                 "InitiateChatForCase",
                 "PutCaseAttributes",
@@ -12319,14 +12321,15 @@
                 "CreateDefaultVpc",
                 "CreateDhcpOptions",
                 "CreateEgressOnlyInternetGateway",
                 "CreateFleet",
                 "CreateFlowLogs",
                 "CreateFpgaImage",
                 "CreateImage",
+                "CreateInstanceConnectEndpoint",
                 "CreateInstanceEventWindow",
                 "CreateInstanceExportTask",
                 "CreateInternetGateway",
                 "CreateIpam",
                 "CreateIpamPool",
                 "CreateIpamResourceDiscovery",
                 "CreateIpamScope",
@@ -12397,14 +12400,15 @@
                 "DeleteCoipPoolPermission",
                 "DeleteCustomerGateway",
                 "DeleteDhcpOptions",
                 "DeleteEgressOnlyInternetGateway",
                 "DeleteFleets",
                 "DeleteFlowLogs",
                 "DeleteFpgaImage",
+                "DeleteInstanceConnectEndpoint",
                 "DeleteInstanceEventWindow",
                 "DeleteInternetGateway",
                 "DeleteIpam",
                 "DeleteIpamPool",
                 "DeleteIpamResourceDiscovery",
                 "DeleteIpamScope",
                 "DeleteKeyPair",
@@ -12513,14 +12517,15 @@
                 "DescribeIdFormat",
                 "DescribeIdentityIdFormat",
                 "DescribeImageAttribute",
                 "DescribeImages",
                 "DescribeImportImageTasks",
                 "DescribeImportSnapshotTasks",
                 "DescribeInstanceAttribute",
+                "DescribeInstanceConnectEndpoints",
                 "DescribeInstanceCreditSpecifications",
                 "DescribeInstanceEventNotificationAttributes",
                 "DescribeInstanceEventWindows",
                 "DescribeInstanceStatus",
                 "DescribeInstanceTypeOfferings",
                 "DescribeInstanceTypes",
                 "DescribeInstances",
```

### Comparing `iam_actions-1.2.20230621/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230622/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999844807250604%*

 * *Differences: {"'ec2'": "{'instance-connect-endpoint': OrderedDict([('arn_pattern', "*

 * *          "'arn:*:ec2:*:*:instance-connect-endpoint/*'), ('condition_keys', "*

 * *          "'aws:RequestTag/${TagKey}')])}"}*

```diff
@@ -1988,14 +1988,18 @@
             "arn_pattern": "arn:*:ec2:*:*:import-snapshot-task/*",
             "condition_keys": "aws:RequestTag/${TagKey}"
         },
         "instance": {
             "arn_pattern": "arn:*:ec2:*:*:instance/*",
             "condition_keys": "aws:RequestTag/${TagKey}"
         },
+        "instance-connect-endpoint": {
+            "arn_pattern": "arn:*:ec2:*:*:instance-connect-endpoint/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
         "instance-event-window": {
             "arn_pattern": "arn:*:ec2:*:*:instance-event-window/*",
             "condition_keys": "aws:RequestTag/${TagKey}"
         },
         "internet-gateway": {
             "arn_pattern": "arn:*:ec2:*:*:internet-gateway/*",
             "condition_keys": "aws:RequestTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230621/iam_actions/services.json` & `iam_actions-1.2.20230622/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999898412244811%*

 * *Differences: {"'ec2'": "{'Actions': {insert: [(72, 'CreateInstanceConnectEndpoint'), (151, "*

 * *          "'DeleteInstanceConnectEndpoint'), (268, 'DescribeInstanceConnectEndpoints')]}}",*

 * * "'support'": "{'Actions': {insert: [(7, 'DescribeCreateCaseOptions'), (12, "*

 * *              "'DescribeSupportedLanguages')]}}"}*

```diff
@@ -6401,14 +6401,15 @@
             "CreateDefaultVpc",
             "CreateDhcpOptions",
             "CreateEgressOnlyInternetGateway",
             "CreateFleet",
             "CreateFlowLogs",
             "CreateFpgaImage",
             "CreateImage",
+            "CreateInstanceConnectEndpoint",
             "CreateInstanceEventWindow",
             "CreateInstanceExportTask",
             "CreateInternetGateway",
             "CreateIpam",
             "CreateIpamPool",
             "CreateIpamResourceDiscovery",
             "CreateIpamScope",
@@ -6479,14 +6480,15 @@
             "DeleteCoipPoolPermission",
             "DeleteCustomerGateway",
             "DeleteDhcpOptions",
             "DeleteEgressOnlyInternetGateway",
             "DeleteFleets",
             "DeleteFlowLogs",
             "DeleteFpgaImage",
+            "DeleteInstanceConnectEndpoint",
             "DeleteInstanceEventWindow",
             "DeleteInternetGateway",
             "DeleteIpam",
             "DeleteIpamPool",
             "DeleteIpamResourceDiscovery",
             "DeleteIpamScope",
             "DeleteKeyPair",
@@ -6595,14 +6597,15 @@
             "DescribeIdFormat",
             "DescribeIdentityIdFormat",
             "DescribeImageAttribute",
             "DescribeImages",
             "DescribeImportImageTasks",
             "DescribeImportSnapshotTasks",
             "DescribeInstanceAttribute",
+            "DescribeInstanceConnectEndpoints",
             "DescribeInstanceCreditSpecifications",
             "DescribeInstanceEventNotificationAttributes",
             "DescribeInstanceEventWindows",
             "DescribeInstanceStatus",
             "DescribeInstanceTypeOfferings",
             "DescribeInstanceTypes",
             "DescribeInstances",
@@ -20010,18 +20013,20 @@
             "AddAttachmentsToSet",
             "AddCommunicationToCase",
             "CreateCase",
             "DescribeAttachment",
             "DescribeCaseAttributes",
             "DescribeCases",
             "DescribeCommunications",
+            "DescribeCreateCaseOptions",
             "DescribeIssueTypes",
             "DescribeServices",
             "DescribeSeverityLevels",
             "DescribeSupportLevel",
+            "DescribeSupportedLanguages",
             "DescribeTrustedAdvisorCheckRefreshStatuses",
             "DescribeTrustedAdvisorCheckResult",
             "DescribeTrustedAdvisorCheckSummaries",
             "DescribeTrustedAdvisorChecks",
             "InitiateCallForCase",
             "InitiateChatForCase",
             "PutCaseAttributes",
```

### Comparing `iam_actions-1.2.20230621/pyproject.toml` & `iam_actions-1.2.20230622/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230621"
+version = "1.2.20230622"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230621/setup.py` & `iam_actions-1.2.20230622/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230621',
+    'version': '1.2.20230622',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230621/PKG-INFO` & `iam_actions-1.2.20230622/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230621
+Version: 1.2.20230622
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

