# Comparing `tmp/datadog_lambda-4.73.0.tar.gz` & `tmp/datadog_lambda-4.74.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog_lambda-4.73.0.tar", max compression
+gzip compressed data, was "datadog_lambda-4.74.0.tar", max compression
```

## Comparing `datadog_lambda-4.73.0.tar` & `datadog_lambda-4.74.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11379 2022-09-22 18:30:00.504292 datadog_lambda-4.73.0/LICENSE
--rw-r--r--   0        0        0      394 2022-09-22 18:30:00.504380 datadog_lambda-4.73.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0     3422 2023-04-18 14:29:41.172896 datadog_lambda-4.73.0/README.md
--rw-r--r--   0        0        0      538 2023-02-13 20:46:09.160997 datadog_lambda-4.73.0/datadog_lambda/__init__.py
--rw-r--r--   0        0        0     3653 2022-09-22 18:30:00.504778 datadog_lambda-4.73.0/datadog_lambda/api.py
--rw-r--r--   0        0        0     7232 2023-04-18 14:29:41.173911 datadog_lambda-4.73.0/datadog_lambda/cold_start.py
--rw-r--r--   0        0        0     1669 2023-01-25 19:31:51.675529 datadog_lambda-4.73.0/datadog_lambda/constants.py
--rw-r--r--   0        0        0     4769 2022-09-22 18:30:00.505031 datadog_lambda-4.73.0/datadog_lambda/dogstatsd.py
--rw-r--r--   0        0        0     1199 2022-09-22 18:30:00.505121 datadog_lambda-4.73.0/datadog_lambda/extension.py
--rw-r--r--   0        0        0      994 2022-09-22 18:30:00.505207 datadog_lambda-4.73.0/datadog_lambda/handler.py
--rw-r--r--   0        0        0     4707 2022-09-22 18:30:00.505343 datadog_lambda-4.73.0/datadog_lambda/metric.py
--rw-r--r--   0        0        0      139 2022-09-22 18:30:00.505417 datadog_lambda-4.73.0/datadog_lambda/module_name.py
--rw-r--r--   0        0        0     4641 2022-09-22 18:30:00.505516 datadog_lambda-4.73.0/datadog_lambda/patch.py
--rw-r--r--   0        0        0      243 2022-09-22 18:30:00.505686 datadog_lambda-4.73.0/datadog_lambda/stats_writer.py
--rw-r--r--   0        0        0      403 2022-09-22 18:30:00.505792 datadog_lambda-4.73.0/datadog_lambda/statsd_writer.py
--rw-r--r--   0        0        0     1751 2022-09-22 18:30:00.505884 datadog_lambda-4.73.0/datadog_lambda/tag_object.py
--rw-r--r--   0        0        0     3240 2022-09-22 18:30:00.505984 datadog_lambda-4.73.0/datadog_lambda/tags.py
--rw-r--r--   0        0        0     2522 2022-09-22 18:30:00.506089 datadog_lambda-4.73.0/datadog_lambda/thread_stats_writer.py
--rw-r--r--   0        0        0    45245 2023-05-24 20:17:42.363176 datadog_lambda-4.73.0/datadog_lambda/tracing.py
--rw-r--r--   0        0        0    12082 2023-04-12 17:19:32.172228 datadog_lambda-4.73.0/datadog_lambda/trigger.py
--rw-r--r--   0        0        0    14126 2023-05-24 20:17:42.363590 datadog_lambda-4.73.0/datadog_lambda/wrapper.py
--rw-r--r--   0        0        0     3449 2023-03-22 12:07:02.672991 datadog_lambda-4.73.0/datadog_lambda/xray.py
--rw-r--r--   0        0        0     1270 2023-05-24 21:34:10.837930 datadog_lambda-4.73.0/pyproject.toml
--rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 datadog_lambda-4.73.0/PKG-INFO
+-rw-r--r--   0        0        0    11379 2023-06-22 16:35:13.671910 datadog_lambda-4.74.0/LICENSE
+-rw-r--r--   0        0        0      394 2023-06-22 16:35:13.671995 datadog_lambda-4.74.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0     3422 2023-06-22 16:35:13.672177 datadog_lambda-4.74.0/README.md
+-rw-r--r--   0        0        0      538 2023-06-22 16:35:13.672315 datadog_lambda-4.74.0/datadog_lambda/__init__.py
+-rw-r--r--   0        0        0     3653 2023-06-22 16:35:13.672408 datadog_lambda-4.74.0/datadog_lambda/api.py
+-rw-r--r--   0        0        0     7232 2023-06-22 16:35:13.672514 datadog_lambda-4.74.0/datadog_lambda/cold_start.py
+-rw-r--r--   0        0        0     1669 2023-06-22 16:35:13.672595 datadog_lambda-4.74.0/datadog_lambda/constants.py
+-rw-r--r--   0        0        0     4769 2023-06-22 16:35:13.672683 datadog_lambda-4.74.0/datadog_lambda/dogstatsd.py
+-rw-r--r--   0        0        0     1199 2023-06-22 16:35:13.672773 datadog_lambda-4.74.0/datadog_lambda/extension.py
+-rw-r--r--   0        0        0      994 2023-06-22 16:35:13.672859 datadog_lambda-4.74.0/datadog_lambda/handler.py
+-rw-r--r--   0        0        0     4707 2023-06-22 16:35:13.672978 datadog_lambda-4.74.0/datadog_lambda/metric.py
+-rw-r--r--   0        0        0      139 2023-06-22 16:35:13.673071 datadog_lambda-4.74.0/datadog_lambda/module_name.py
+-rw-r--r--   0        0        0     4641 2023-06-22 16:35:13.673170 datadog_lambda-4.74.0/datadog_lambda/patch.py
+-rw-r--r--   0        0        0      243 2023-06-22 16:35:13.673254 datadog_lambda-4.74.0/datadog_lambda/stats_writer.py
+-rw-r--r--   0        0        0      403 2023-06-22 16:35:13.673338 datadog_lambda-4.74.0/datadog_lambda/statsd_writer.py
+-rw-r--r--   0        0        0     1751 2023-06-22 16:35:13.673428 datadog_lambda-4.74.0/datadog_lambda/tag_object.py
+-rw-r--r--   0        0        0     3240 2023-06-22 16:35:13.673544 datadog_lambda-4.74.0/datadog_lambda/tags.py
+-rw-r--r--   0        0        0     2522 2023-06-22 16:35:13.673636 datadog_lambda-4.74.0/datadog_lambda/thread_stats_writer.py
+-rw-r--r--   0        0        0    47208 2023-06-22 16:35:13.673836 datadog_lambda-4.74.0/datadog_lambda/tracing.py
+-rw-r--r--   0        0        0    12082 2023-06-22 16:35:13.673975 datadog_lambda-4.74.0/datadog_lambda/trigger.py
+-rw-r--r--   0        0        0    14242 2023-06-22 16:35:13.674085 datadog_lambda-4.74.0/datadog_lambda/wrapper.py
+-rw-r--r--   0        0        0     3449 2023-06-22 16:35:13.674183 datadog_lambda-4.74.0/datadog_lambda/xray.py
+-rw-r--r--   0        0        0     1271 2023-06-22 16:41:53.033918 datadog_lambda-4.74.0/pyproject.toml
+-rw-r--r--   0        0        0     5002 1970-01-01 00:00:00.000000 datadog_lambda-4.74.0/PKG-INFO
```

### Comparing `datadog_lambda-4.73.0/LICENSE` & `datadog_lambda-4.74.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/README.md` & `datadog_lambda-4.74.0/README.md`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/__init__.py` & `datadog_lambda-4.74.0/datadog_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/api.py` & `datadog_lambda-4.74.0/datadog_lambda/api.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/cold_start.py` & `datadog_lambda-4.74.0/datadog_lambda/cold_start.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/constants.py` & `datadog_lambda-4.74.0/datadog_lambda/constants.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/dogstatsd.py` & `datadog_lambda-4.74.0/datadog_lambda/dogstatsd.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/extension.py` & `datadog_lambda-4.74.0/datadog_lambda/extension.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/handler.py` & `datadog_lambda-4.74.0/datadog_lambda/handler.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/metric.py` & `datadog_lambda-4.74.0/datadog_lambda/metric.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/patch.py` & `datadog_lambda-4.74.0/datadog_lambda/patch.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/tag_object.py` & `datadog_lambda-4.74.0/datadog_lambda/tag_object.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/tags.py` & `datadog_lambda-4.74.0/datadog_lambda/tags.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/thread_stats_writer.py` & `datadog_lambda-4.74.0/datadog_lambda/thread_stats_writer.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/tracing.py` & `datadog_lambda-4.74.0/datadog_lambda/tracing.py`

 * *Files 4% similar despite different names*

```diff
@@ -680,31 +680,58 @@
             e,
         )
         return None
     logger.debug("Unable to infer a span: unknown event type")
     return None
 
 
+def create_service_mapping(val):
+    new_service_mapping = {}
+    for entry in val.split(","):
+        parts = entry.split(":")
+        if len(parts) == 2:
+            key = parts[0].strip()
+            value = parts[1].strip()
+            if key != value and key and value:
+                new_service_mapping[key] = value
+    return new_service_mapping
+
+
+def determine_service_name(service_mapping, specific_key, generic_key, default_value):
+    service_name = service_mapping.get(specific_key)
+    if service_name is None:
+        service_name = service_mapping.get(generic_key, default_value)
+    return service_name
+
+
+service_mapping = {}
+# Initialization code
+service_mapping_str = os.getenv("DD_SERVICE_MAPPING", "")
+service_mapping = create_service_mapping(service_mapping_str)
+
+
 def create_inferred_span_from_lambda_function_url_event(event, context):
     request_context = event.get("requestContext")
+    api_id = request_context.get("apiId")
     domain = request_context.get("domainName")
+    service_name = determine_service_name(service_mapping, api_id, "lambda_url", domain)
     method = request_context.get("http", {}).get("method")
     path = request_context.get("http", {}).get("path")
     resource = "{0} {1}".format(method, path)
     tags = {
         "operation_name": "aws.lambda.url",
         "http.url": domain + path,
         "endpoint": path,
         "http.method": method,
         "resource_names": domain + path,
         "request_id": context.aws_request_id,
     }
     request_time_epoch = request_context.get("timeEpoch")
     args = {
-        "service": domain,
+        "service": service_name,
         "resource": resource,
         "span_type": "http",
     }
     tracer.set_tags(
         {"_dd.origin": "lambda"}
     )  # function urls don't count as lambda_inferred,
     # because they're in the same service as the inferring lambda function
@@ -785,34 +812,39 @@
 
 def create_inferred_span_from_api_gateway_websocket_event(
     event, context, decode_authorizer_context: bool = True
 ):
     request_context = event.get("requestContext")
     domain = request_context.get("domainName")
     endpoint = request_context.get("routeKey")
+    api_id = request_context.get("apiId")
+
+    service_name = determine_service_name(
+        service_mapping, api_id, "lambda_api_gateway", domain
+    )
     tags = {
         "operation_name": "aws.apigateway.websocket",
         "http.url": domain + endpoint,
         "endpoint": endpoint,
         "resource_names": endpoint,
-        "apiid": request_context.get("apiId"),
-        "apiname": request_context.get("apiId"),
+        "apiid": api_id,
+        "apiname": api_id,
         "stage": request_context.get("stage"),
         "request_id": context.aws_request_id,
         "connection_id": request_context.get("connectionId"),
         "event_type": request_context.get("eventType"),
         "message_direction": request_context.get("messageDirection"),
     }
     request_time_epoch_ms = int(request_context.get("requestTimeEpoch"))
     if is_api_gateway_invocation_async(event):
         InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="async")
     else:
         InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="sync")
     args = {
-        "service": domain,
+        "service": service_name,
         "resource": endpoint,
         "span_type": "web",
     }
     tracer.set_tags({"_dd.origin": "lambda"})
     upstream_authorizer_span = None
     finish_time_ns = None
     if decode_authorizer_context:
@@ -833,35 +865,39 @@
 
 
 def create_inferred_span_from_api_gateway_event(
     event, context, decode_authorizer_context: bool = True
 ):
     request_context = event.get("requestContext")
     domain = request_context.get("domainName", "")
+    api_id = request_context.get("apiId")
+    service_name = determine_service_name(
+        service_mapping, api_id, "lambda_api_gateway", domain
+    )
     method = event.get("httpMethod")
     path = event.get("path")
     resource = "{0} {1}".format(method, path)
     tags = {
         "operation_name": "aws.apigateway.rest",
         "http.url": domain + path,
         "endpoint": path,
         "http.method": method,
         "resource_names": resource,
-        "apiid": request_context.get("apiId"),
-        "apiname": request_context.get("apiId"),
+        "apiid": api_id,
+        "apiname": api_id,
         "stage": request_context.get("stage"),
         "request_id": context.aws_request_id,
     }
     request_time_epoch_ms = int(request_context.get("requestTimeEpoch"))
     if is_api_gateway_invocation_async(event):
         InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="async")
     else:
         InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="sync")
     args = {
-        "service": domain,
+        "service": service_name,
         "resource": resource,
         "span_type": "http",
     }
     tracer.set_tags({"_dd.origin": "lambda"})
     upstream_authorizer_span = None
     finish_time_ns = None
     if decode_authorizer_context:
@@ -883,38 +919,42 @@
 
 
 def create_inferred_span_from_http_api_event(
     event, context, decode_authorizer_context: bool = True
 ):
     request_context = event.get("requestContext")
     domain = request_context.get("domainName")
+    api_id = request_context.get("apiId")
+    service_name = determine_service_name(
+        service_mapping, api_id, "lambda_api_gateway", domain
+    )
     method = request_context.get("http", {}).get("method")
     path = event.get("rawPath")
     resource = "{0} {1}".format(method, path)
     tags = {
         "operation_name": "aws.httpapi",
         "endpoint": path,
         "http.url": domain + path,
         "http.method": request_context.get("http", {}).get("method"),
         "http.protocol": request_context.get("http", {}).get("protocol"),
         "http.source_ip": request_context.get("http", {}).get("sourceIp"),
         "http.user_agent": request_context.get("http", {}).get("userAgent"),
         "resource_names": resource,
         "request_id": context.aws_request_id,
-        "apiid": request_context.get("apiId"),
-        "apiname": request_context.get("apiId"),
+        "apiid": api_id,
+        "apiname": api_id,
         "stage": request_context.get("stage"),
     }
     request_time_epoch_ms = int(request_context.get("timeEpoch"))
     if is_api_gateway_invocation_async(event):
         InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="async")
     else:
         InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="sync")
     args = {
-        "service": domain,
+        "service": service_name,
         "resource": resource,
         "span_type": "http",
     }
     tracer.set_tags({"_dd.origin": "lambda"})
     inferred_span_start_ns = request_time_epoch_ms * 1e6
     if decode_authorizer_context:
         injected_authorizer_data = get_injected_authorizer_data(event, True)
@@ -931,26 +971,29 @@
 
 def create_inferred_span_from_sqs_event(event, context):
     trace_ctx = tracer.current_trace_context()
 
     event_record = get_first_record(event)
     event_source_arn = event_record.get("eventSourceARN")
     queue_name = event_source_arn.split(":")[-1]
+    service_name = determine_service_name(
+        service_mapping, queue_name, "lambda_sqs", "sqs"
+    )
     tags = {
         "operation_name": "aws.sqs",
         "resource_names": queue_name,
         "queuename": queue_name,
         "event_source_arn": event_source_arn,
         "receipt_handle": event_record.get("receiptHandle"),
         "sender_id": event_record.get("attributes", {}).get("SenderId"),
     }
     InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="async")
     request_time_epoch = event_record.get("attributes", {}).get("SentTimestamp")
     args = {
-        "service": "sqs",
+        "service": service_name,
         "resource": queue_name,
         "span_type": "web",
     }
     start_time = int(request_time_epoch) / 1000
 
     # logic to deal with SNS => SQS event
     sns_span = None
@@ -985,14 +1028,17 @@
 
 
 def create_inferred_span_from_sns_event(event, context):
     event_record = get_first_record(event)
     sns_message = event_record.get("Sns")
     topic_arn = event_record.get("Sns", {}).get("TopicArn")
     topic_name = topic_arn.split(":")[-1]
+    service_name = determine_service_name(
+        service_mapping, topic_name, "lambda_sns", "sns"
+    )
     tags = {
         "operation_name": "aws.sns",
         "resource_names": topic_name,
         "topicname": topic_name,
         "topic_arn": topic_arn,
         "message_id": sns_message.get("MessageId"),
         "type": sns_message.get("Type"),
@@ -1004,15 +1050,15 @@
 
     InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="async")
     sns_dt_format = "%Y-%m-%dT%H:%M:%S.%fZ"
     timestamp = event_record.get("Sns", {}).get("Timestamp")
     dt = datetime.strptime(timestamp, sns_dt_format)
 
     args = {
-        "service": "sns",
+        "service": service_name,
         "resource": topic_name,
         "span_type": "web",
     }
     tracer.set_tags({"_dd.origin": "lambda"})
     span = tracer.trace("aws.sns", **args)
     if span:
         span.set_tags(tags)
@@ -1022,14 +1068,17 @@
 
 def create_inferred_span_from_kinesis_event(event, context):
     event_record = get_first_record(event)
     event_source_arn = event_record.get("eventSourceARN")
     event_id = event_record.get("eventID")
     stream_name = event_source_arn.split(":")[-1]
     shard_id = event_id.split(":")[0]
+    service_name = determine_service_name(
+        service_mapping, stream_name, "lambda_kinesis", "kinesis"
+    )
     tags = {
         "operation_name": "aws.kinesis",
         "resource_names": stream_name,
         "streamname": stream_name,
         "shardid": shard_id,
         "event_source_arn": event_source_arn,
         "event_id": event_id,
@@ -1039,15 +1088,15 @@
     }
     InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="async")
     request_time_epoch = event_record.get("kinesis", {}).get(
         "approximateArrivalTimestamp"
     )
 
     args = {
-        "service": "kinesis",
+        "service": service_name,
         "resource": stream_name,
         "span_type": "web",
     }
     tracer.set_tags({"_dd.origin": "lambda"})
     span = tracer.trace("aws.kinesis", **args)
     if span:
         span.set_tags(tags)
@@ -1055,14 +1104,17 @@
     return span
 
 
 def create_inferred_span_from_dynamodb_event(event, context):
     event_record = get_first_record(event)
     event_source_arn = event_record.get("eventSourceARN")
     table_name = event_source_arn.split("/")[1]
+    service_name = determine_service_name(
+        service_mapping, table_name, "lambda_dynamodb", "dynamodb"
+    )
     dynamodb_message = event_record.get("dynamodb")
     tags = {
         "operation_name": "aws.dynamodb",
         "resource_names": table_name,
         "tablename": table_name,
         "event_source_arn": event_source_arn,
         "event_id": event_record.get("eventID"),
@@ -1072,15 +1124,15 @@
         "size_bytes": str(dynamodb_message.get("SizeBytes")),
     }
     InferredSpanInfo.set_tags(tags, synchronicity="async", tag_source="self")
     request_time_epoch = event_record.get("dynamodb", {}).get(
         "ApproximateCreationDateTime"
     )
     args = {
-        "service": "dynamodb",
+        "service": service_name,
         "resource": table_name,
         "span_type": "web",
     }
     tracer.set_tags({"_dd.origin": "lambda"})
     span = tracer.trace("aws.dynamodb", **args)
     if span:
         span.set_tags(tags)
@@ -1088,14 +1140,17 @@
     span.start = int(request_time_epoch)
     return span
 
 
 def create_inferred_span_from_s3_event(event, context):
     event_record = get_first_record(event)
     bucket_name = event_record.get("s3", {}).get("bucket", {}).get("name")
+    service_name = determine_service_name(
+        service_mapping, bucket_name, "lambda_s3", "s3"
+    )
     tags = {
         "operation_name": "aws.s3",
         "resource_names": bucket_name,
         "event_name": event_record.get("eventName"),
         "bucketname": bucket_name,
         "bucket_arn": event_record.get("s3", {}).get("bucket", {}).get("arn"),
         "object_key": event_record.get("s3", {}).get("object", {}).get("key"),
@@ -1104,28 +1159,31 @@
     }
     InferredSpanInfo.set_tags(tags, synchronicity="async", tag_source="self")
     dt_format = "%Y-%m-%dT%H:%M:%S.%fZ"
     timestamp = event_record.get("eventTime")
     dt = datetime.strptime(timestamp, dt_format)
 
     args = {
-        "service": "s3",
+        "service": service_name,
         "resource": bucket_name,
         "span_type": "web",
     }
     tracer.set_tags({"_dd.origin": "lambda"})
     span = tracer.trace("aws.s3", **args)
     if span:
         span.set_tags(tags)
     span.start = dt.replace(tzinfo=timezone.utc).timestamp()
     return span
 
 
 def create_inferred_span_from_eventbridge_event(event, context):
     source = event.get("source")
+    service_name = determine_service_name(
+        service_mapping, source, "lambda_eventbridge", "eventbridge"
+    )
     tags = {
         "operation_name": "aws.eventbridge",
         "resource_names": source,
         "detail_type": event.get("detail-type"),
     }
     InferredSpanInfo.set_tags(
         tags,
@@ -1133,15 +1191,15 @@
         tag_source="self",
     )
     dt_format = "%Y-%m-%dT%H:%M:%SZ"
     timestamp = event.get("time")
     dt = datetime.strptime(timestamp, dt_format)
 
     args = {
-        "service": "eventbridge",
+        "service": service_name,
         "resource": source,
         "span_type": "web",
     }
     tracer.set_tags({"_dd.origin": "lambda"})
     span = tracer.trace("aws.eventbridge", **args)
     if span:
         span.set_tags(tags)
```

### Comparing `datadog_lambda-4.73.0/datadog_lambda/trigger.py` & `datadog_lambda-4.74.0/datadog_lambda/trigger.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/datadog_lambda/wrapper.py` & `datadog_lambda-4.74.0/datadog_lambda/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,30 +50,31 @@
     from ddtrace.profiling import profiler
 
 logger = logging.getLogger(__name__)
 
 dd_capture_lambda_payload_enabled = (
     os.environ.get("DD_CAPTURE_LAMBDA_PAYLOAD", "false").lower() == "true"
 )
-service_env_var = os.environ.get("DD_SERVICE", "DefaultServiceName")
-env_env_var = os.environ.get("DD_ENV", None)
 
 DD_FLUSH_TO_LOG = "DD_FLUSH_TO_LOG"
 DD_LOGS_INJECTION = "DD_LOGS_INJECTION"
 DD_MERGE_XRAY_TRACES = "DD_MERGE_XRAY_TRACES"
 AWS_LAMBDA_FUNCTION_NAME = "AWS_LAMBDA_FUNCTION_NAME"
 DD_TRACE_EXTRACTOR = "DD_TRACE_EXTRACTOR"
 DD_TRACE_MANAGED_SERVICES = "DD_TRACE_MANAGED_SERVICES"
 DD_ENCODE_AUTHORIZER_CONTEXT = "DD_ENCODE_AUTHORIZER_CONTEXT"
 DD_DECODE_AUTHORIZER_CONTEXT = "DD_DECODE_AUTHORIZER_CONTEXT"
 DD_COLD_START_TRACING = "DD_COLD_START_TRACING"
 DD_MIN_COLD_START_DURATION = "DD_MIN_COLD_START_DURATION"
 DD_COLD_START_TRACE_SKIP_LIB = "DD_COLD_START_TRACE_SKIP_LIB"
 DD_REQUESTS_SERVICE_NAME = "DD_REQUESTS_SERVICE_NAME"
 DD_SERVICE = "DD_SERVICE"
+DD_ENV = "DD_ENV"
+
+env_env_var = os.environ.get(DD_ENV, None)
 
 """
 Usage:
 
 import requests
 from datadog_lambda.wrapper import datadog_lambda_wrapper
 from datadog_lambda.metric import lambda_metric
@@ -128,14 +129,15 @@
             self.logs_injection = (
                 os.environ.get(DD_LOGS_INJECTION, "true").lower() == "true"
             )
             self.merge_xray_traces = (
                 os.environ.get(DD_MERGE_XRAY_TRACES, "false").lower() == "true"
             )
             self.function_name = os.environ.get(AWS_LAMBDA_FUNCTION_NAME, "function")
+            self.service = os.environ.get(DD_SERVICE, None)
             self.extractor_env = os.environ.get(DD_TRACE_EXTRACTOR, None)
             self.trace_extractor = None
             self.span = None
             self.inferred_span = None
             depends_on_dd_tracing_enabled = (
                 lambda original_boolean: dd_tracing_enabled and original_boolean
             )
@@ -168,15 +170,15 @@
                     self.cold_start_trace_skip_lib = os.environ[
                         DD_COLD_START_TRACE_SKIP_LIB
                     ].split(",")
                 except Exception:
                     logger.debug(f"Malformatted for env {DD_COLD_START_TRACE_SKIP_LIB}")
             self.response = None
             if profiling_env_var:
-                self.prof = profiler.Profiler(env=env_env_var, service=service_env_var)
+                self.prof = profiler.Profiler(env=env_env_var, service=self.service)
             if self.extractor_env:
                 extractor_parts = self.extractor_env.rsplit(".", 1)
                 if len(extractor_parts) == 2:
                     (mod_name, extractor_name) = extractor_parts
                     modified_extractor_name = modify_module_name(mod_name)
                     extractor_module = import_module(modified_extractor_name)
                     self.trace_extractor = getattr(extractor_module, extractor_name)
@@ -311,14 +313,17 @@
                     self.span.set_tag("http.status_code", status_code)
                 self.span.finish()
 
             if self.inferred_span:
                 if status_code:
                     self.inferred_span.set_tag("http.status_code", status_code)
 
+                if self.service:
+                    self.inferred_span.set_tag("peer.service", self.service)
+
                 if InferredSpanInfo.is_async(self.inferred_span) and self.span:
                     self.inferred_span.finish(finish_time=self.span.start)
                 else:
                     self.inferred_span.finish()
 
             if should_trace_cold_start:
                 try:
```

### Comparing `datadog_lambda-4.73.0/datadog_lambda/xray.py` & `datadog_lambda-4.74.0/datadog_lambda/xray.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.73.0/pyproject.toml` & `datadog_lambda-4.74.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datadog_lambda"
-version = "4.73.0"
+version = "4.74.0"
 description = "The Datadog AWS Lambda Library"
 authors = ["Datadog, Inc. <dev@datadoghq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/DataDog/datadog-lambda-python"
 keywords = [
     "datadog",
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 datadog = ">=0.41.0,<1.0.0"
 wrapt = "^1.11.2"
-ddtrace = "^1.6.4"
+ddtrace = "^1.15.0"
 urllib3 = "<2.0.0"
 importlib_metadata = {version = "^1.0", python = "<3.8"}
 boto3 = { version = "^1.10.33", optional = true }
 typing_extensions = {version = "^4.0", python = "<3.8"}
 requests = { version ="^2.22.0", optional = true }
 nose2 = { version= "^0.9.1", optional = true }
 flake8 = { version = "^3.7.9", optional = true }
```

### Comparing `datadog_lambda-4.73.0/PKG-INFO` & `datadog_lambda-4.74.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: datadog-lambda
-Version: 4.73.0
+Version: 4.74.0
 Summary: The Datadog AWS Lambda Library
 Home-page: https://github.com/DataDog/datadog-lambda-python
 License: Apache-2.0
 Keywords: datadog,aws,lambda,layer
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 Requires-Python: >=3.7.0,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Requires-Dist: boto3 (>=1.10.33,<2.0.0) ; extra == "dev"
 Requires-Dist: datadog (>=0.41.0,<1.0.0)
-Requires-Dist: ddtrace (>=1.6.4,<2.0.0)
+Requires-Dist: ddtrace (>=1.15.0,<2.0.0)
 Requires-Dist: flake8 (>=3.7.9,<4.0.0) ; extra == "dev"
 Requires-Dist: httpretty (>=0.9.7,<0.10.0) ; extra == "dev"
 Requires-Dist: importlib_metadata (>=1.0,<2.0) ; python_version < "3.8"
 Requires-Dist: nose2 (>=0.9.1,<0.10.0) ; extra == "dev"
 Requires-Dist: requests (>=2.22.0,<3.0.0) ; extra == "dev"
 Requires-Dist: typing_extensions (>=4.0,<5.0) ; python_version < "3.8"
 Requires-Dist: urllib3 (<2.0.0)
```

