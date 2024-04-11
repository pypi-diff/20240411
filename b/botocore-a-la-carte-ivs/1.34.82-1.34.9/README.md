# Comparing `tmp/botocore-a-la-carte-ivs-1.34.82.tar.gz` & `tmp/botocore-a-la-carte-ivs-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ivs-1.34.82.tar", last modified: Thu Apr 11 01:00:53 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-ivs-1.34.9.tar", last modified: Thu Dec 28 01:06:46 2023, max compression
```

## Comparing `botocore-a-la-carte-ivs-1.34.82.tar` & `botocore-a-la-carte-ivs-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:53.536802 botocore-a-la-carte-ivs-1.34.82/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-11 01:00:53.000000 botocore-a-la-carte-ivs-1.34.82/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-11 01:00:53.536802 botocore-a-la-carte-ivs-1.34.82/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:53.536802 botocore-a-la-carte-ivs-1.34.82/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:53.536802 botocore-a-la-carte-ivs-1.34.82/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:53.536802 botocore-a-la-carte-ivs-1.34.82/botocore/data/ivs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:53.536802 botocore-a-la-carte-ivs-1.34.82/botocore/data/ivs/2020-07-14/
--rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-11 01:00:33.000000 botocore-a-la-carte-ivs-1.34.82/botocore/data/ivs/2020-07-14/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 01:00:33.000000 botocore-a-la-carte-ivs-1.34.82/botocore/data/ivs/2020-07-14/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-11 01:00:33.000000 botocore-a-la-carte-ivs-1.34.82/botocore/data/ivs/2020-07-14/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   120243 2024-04-11 01:00:33.000000 botocore-a-la-carte-ivs-1.34.82/botocore/data/ivs/2020-07-14/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:53.536802 botocore-a-la-carte-ivs-1.34.82/botocore_a_la_carte_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-11 01:00:53.000000 botocore-a-la-carte-ivs-1.34.82/botocore_a_la_carte_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-11 01:00:53.000000 botocore-a-la-carte-ivs-1.34.82/botocore_a_la_carte_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:00:53.000000 botocore-a-la-carte-ivs-1.34.82/botocore_a_la_carte_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 01:00:53.000000 botocore-a-la-carte-ivs-1.34.82/botocore_a_la_carte_ivs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 01:00:53.536802 botocore-a-la-carte-ivs-1.34.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-11 01:00:53.000000 botocore-a-la-carte-ivs-1.34.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.218314 botocore-a-la-carte-ivs-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:45.000000 botocore-a-la-carte-ivs-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:06:46.218314 botocore-a-la-carte-ivs-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.214314 botocore-a-la-carte-ivs-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.214314 botocore-a-la-carte-ivs-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.214314 botocore-a-la-carte-ivs-1.34.9/botocore/data/ivs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.214314 botocore-a-la-carte-ivs-1.34.9/botocore/data/ivs/2020-07-14/
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2023-12-28 01:06:26.000000 botocore-a-la-carte-ivs-1.34.9/botocore/data/ivs/2020-07-14/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-ivs-1.34.9/botocore/data/ivs/2020-07-14/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2023-12-28 01:06:26.000000 botocore-a-la-carte-ivs-1.34.9/botocore/data/ivs/2020-07-14/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   102689 2023-12-28 01:06:26.000000 botocore-a-la-carte-ivs-1.34.9/botocore/data/ivs/2020-07-14/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.218314 botocore-a-la-carte-ivs-1.34.9/botocore_a_la_carte_ivs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:06:46.000000 botocore-a-la-carte-ivs-1.34.9/botocore_a_la_carte_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-28 01:06:46.000000 botocore-a-la-carte-ivs-1.34.9/botocore_a_la_carte_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:46.000000 botocore-a-la-carte-ivs-1.34.9/botocore_a_la_carte_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:46.000000 botocore-a-la-carte-ivs-1.34.9/botocore_a_la_carte_ivs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:46.218314 botocore-a-la-carte-ivs-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-12-28 01:06:45.000000 botocore-a-la-carte-ivs-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-ivs-1.34.82/LICENSE.txt` & `botocore-a-la-carte-ivs-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ivs-1.34.82/PKG-INFO` & `botocore-a-la-carte-ivs-1.34.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ivs
-Version: 1.34.82
+Version: 1.34.9
 Summary: ivs data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ivs-1.34.82/botocore/data/ivs/2020-07-14/endpoint-rule-set-1.json` & `botocore-a-la-carte-ivs-1.34.9/botocore/data/ivs/2020-07-14/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ivs-1.34.82/botocore/data/ivs/2020-07-14/paginators-1.json` & `botocore-a-la-carte-ivs-1.34.9/botocore/data/ivs/2020-07-14/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ivs-1.34.82/botocore/data/ivs/2020-07-14/service-2.json` & `botocore-a-la-carte-ivs-1.34.9/botocore/data/ivs/2020-07-14/service-2.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8724639985637582%*

 * *Differences: {"'documentation'": "'<p> <b>Introduction</b> </p> <p>The Amazon Interactive Video Service (IVS) "*

 * *                    'API is REST compatible, using a standard HTTP API and an Amazon Web Services '*

 * *                    'EventBridge event stream for responses. JSON is used for both requests and '*

 * *                    'responses, including errors.</p> <p>The API is an Amazon Web Services '*

 * *                    'regional service. For a list of supported regions and Amazon IVS HTTPS '*

 * *                    'service […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "documentation": "<p> <b>Introduction</b> </p> <p>The Amazon Interactive Video Service (IVS) API is REST compatible, using a standard HTTP API and an Amazon Web Services EventBridge event stream for responses. JSON is used for both requests and responses, including errors.</p> <p>The API is an Amazon Web Services regional service. For a list of supported regions and Amazon IVS HTTPS service endpoints, see the <a href=\"https://docs.aws.amazon.com/general/latest/gr/ivs.html\">Amazon IVS page</a> in the <i>Amazon Web Services General Reference</i>.</p> <p> <i> <b>All API request parameters and URLs are case sensitive. </b> </i> </p> <p>For a summary of notable documentation changes in each release, see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/doc-history.html\"> Document History</a>.</p> <p> <b>Allowed Header Values</b> </p> <ul> <li> <p> <code> <b>Accept:</b> </code> application/json</p> </li> <li> <p> <code> <b>Accept-Encoding:</b> </code> gzip, deflate</p> </li> <li> <p> <code> <b>Content-Type:</b> </code>application/json</p> </li> </ul> <p> <b>Key Concepts</b> </p> <ul> <li> <p> <b>Channel</b> \u2014 Stores configuration data related to your live stream. You first create a channel and then use the channel\u2019s stream key to start your live stream.</p> </li> <li> <p> <b>Stream key</b> \u2014 An identifier assigned by Amazon IVS when you create a channel, which is then used to authorize streaming. <i> <b>Treat the stream key like a secret, since it allows anyone to stream to the channel.</b> </i> </p> </li> <li> <p> <b>Playback key pair</b> \u2014 Video playback may be restricted using playback-authorization tokens, which use public-key encryption. A playback key pair is the public-private pair of keys used to sign and validate the playback-authorization token.</p> </li> <li> <p> <b>Recording configuration</b> \u2014 Stores configuration related to recording a live stream and where to store the recorded content. Multiple channels can reference the same recording configuration.</p> </li> <li> <p> <b>Playback restriction policy</b> \u2014 Restricts playback by countries and/or origin sites.</p> </li> </ul> <p>For more information about your IVS live stream, also see <a href=\"https://docs.aws.amazon.com/ivs/latest/LowLatencyUserGuide/getting-started.html\">Getting Started with IVS Low-Latency Streaming</a>.</p> <p> <b>Tagging</b> </p> <p>A <i>tag</i> is a metadata label that you assign to an Amazon Web Services resource. A tag comprises a <i>key</i> and a <i>value</i>, both set by you. For example, you might set a tag as <code>topic:nature</code> to label a particular video category. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p> <p>Tags can help you identify and organize your Amazon Web Services resources. For example, you can use the same tag for different resources to indicate that they are related. You can also use tags to manage access (see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_tags.html\"> Access Tags</a>). </p> <p>The Amazon IVS API has these tag-related endpoints: <a>TagResource</a>, <a>UntagResource</a>, and <a>ListTagsForResource</a>. The following resources support tagging: Channels, Stream Keys, Playback Key Pairs, and Recording Configurations.</p> <p>At most 50 tags can be applied to a resource. </p> <p> <b>Authentication versus Authorization</b> </p> <p>Note the differences between these concepts:</p> <ul> <li> <p> <i>Authentication</i> is about verifying identity. You need to be authenticated to sign Amazon IVS API requests.</p> </li> <li> <p> <i>Authorization</i> is about granting permissions. Your IAM roles need to have permissions for Amazon IVS API requests. In addition, authorization is needed to view <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/private-channels.html\">Amazon IVS private channels</a>. (Private channels are channels that are enabled for \"playback authorization.\")</p> </li> </ul> <p> <b>Authentication</b> </p> <p>All Amazon IVS API requests must be authenticated with a signature. The Amazon Web Services Command-Line Interface (CLI) and Amazon IVS Player SDKs take care of signing the underlying API calls for you. However, if your application calls the Amazon IVS API directly, it\u2019s your responsibility to sign the requests.</p> <p>You generate a signature using valid Amazon Web Services credentials that have permission to perform the requested action. For example, you must sign PutMetadata requests with a signature generated from a user account that has the <code>ivs:PutMetadata</code> permission.</p> <p>For more information:</p> <ul> <li> <p>Authentication and generating signatures \u2014 See <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/sig-v4-authenticating-requests.html\">Authenticating Requests (Amazon Web Services Signature Version 4)</a> in the <i>Amazon Web Services General Reference</i>.</p> </li> <li> <p>Managing Amazon IVS permissions \u2014 See <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/security-iam.html\">Identity and Access Management</a> on the Security page of the <i>Amazon IVS User Guide</i>.</p> </li> </ul> <p> <b>Amazon Resource Names (ARNs)</b> </p> <p>ARNs uniquely identify AWS resources. An ARN is required when you need to specify a resource unambiguously across all of AWS, such as in IAM policies and API calls. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\">Amazon Resource Names</a> in the <i>AWS General Reference</i>.</p> <p> <b>Channel Endpoints</b> </p> <ul> <li> <p> <a>CreateChannel</a> \u2014 Creates a new channel and an associated stream key to start streaming.</p> </li> <li> <p> <a>GetChannel</a> \u2014 Gets the channel configuration for the specified channel ARN.</p> </li> <li> <p> <a>BatchGetChannel</a> \u2014 Performs <a>GetChannel</a> on multiple ARNs simultaneously.</p> </li> <li> <p> <a>ListChannels</a> \u2014 Gets summary information about all channels in your account, in the Amazon Web Services region where the API request is processed. This list can be filtered to match a specified name or recording-configuration ARN. Filters are mutually exclusive and cannot be used together. If you try to use both filters, you will get an error (409 Conflict Exception).</p> </li> <li> <p> <a>UpdateChannel</a> \u2014 Updates a channel's configuration. This does not affect an ongoing stream of this channel. You must stop and restart the stream for the changes to take effect.</p> </li> <li> <p> <a>DeleteChannel</a> \u2014 Deletes the specified channel.</p> </li> </ul> <p> <b>Playback Restriction Policy Endpoints</b> </p> <ul> <li> <p> <a>CreatePlaybackRestrictionPolicy</a> \u2014 Creates a new playback restriction policy, for constraining playback by countries and/or origins.</p> </li> <li> <p> <a>DeletePlaybackRestrictionPolicy</a> \u2014 Deletes the specified playback restriction policy</p> </li> <li> <p> <a>GetPlaybackRestrictionPolicy</a> \u2014 Gets the specified playback restriction policy.</p> </li> <li> <p> <a>ListPlaybackRestrictionPolicies</a> \u2014 Gets summary information about playback restriction policies.</p> </li> <li> <p> <a>UpdatePlaybackRestrictionPolicy</a> \u2014 Updates a specified playback restriction policy.</p> </li> </ul> <p> <b>Private Channel Endpoints</b> </p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/private-channels.html\">Setting Up Private Channels</a> in the <i>Amazon IVS User Guide</i>.</p> <ul> <li> <p> <a>ImportPlaybackKeyPair</a> \u2014 Imports the public portion of a new key pair and returns its <code>arn</code> and <code>fingerprint</code>. The <code>privateKey</code> can then be used to generate viewer authorization tokens, to grant viewers access to private channels (channels enabled for playback authorization).</p> </li> <li> <p> <a>GetPlaybackKeyPair</a> \u2014 Gets a specified playback authorization key pair and returns the <code>arn</code> and <code>fingerprint</code>. The <code>privateKey</code> held by the caller can be used to generate viewer authorization tokens, to grant viewers access to private channels.</p> </li> <li> <p> <a>ListPlaybackKeyPairs</a> \u2014 Gets summary information about playback key pairs.</p> </li> <li> <p> <a>DeletePlaybackKeyPair</a> \u2014 Deletes a specified authorization key pair. This invalidates future viewer tokens generated using the key pair\u2019s <code>privateKey</code>.</p> </li> <li> <p> <a>StartViewerSessionRevocation</a> \u2014 Starts the process of revoking the viewer session associated with a specified channel ARN and viewer ID. Optionally, you can provide a version to revoke viewer sessions less than and including that version.</p> </li> <li> <p> <a>BatchStartViewerSessionRevocation</a> \u2014 Performs <a>StartViewerSessionRevocation</a> on multiple channel ARN and viewer ID pairs simultaneously.</p> </li> </ul> <p> <b>Recording Configuration Endpoints</b> </p> <ul> <li> <p> <a>CreateRecordingConfiguration</a> \u2014 Creates a new recording configuration, used to enable recording to Amazon S3.</p> </li> <li> <p> <a>GetRecordingConfiguration</a> \u2014 Gets the recording-configuration metadata for the specified ARN.</p> </li> <li> <p> <a>ListRecordingConfigurations</a> \u2014 Gets summary information about all recording configurations in your account, in the Amazon Web Services region where the API request is processed.</p> </li> <li> <p> <a>DeleteRecordingConfiguration</a> \u2014 Deletes the recording configuration for the specified ARN.</p> </li> </ul> <p> <b>Stream Endpoints</b> </p> <ul> <li> <p> <a>GetStream</a> \u2014 Gets information about the active (live) stream on a specified channel.</p> </li> <li> <p> <a>GetStreamSession</a> \u2014 Gets metadata on a specified stream.</p> </li> <li> <p> <a>ListStreams</a> \u2014 Gets summary information about live streams in your account, in the Amazon Web Services region where the API request is processed.</p> </li> <li> <p> <a>ListStreamSessions</a> \u2014 Gets a summary of current and previous streams for a specified channel in your account, in the AWS region where the API request is processed.</p> </li> <li> <p> <a>StopStream</a> \u2014 Disconnects the incoming RTMPS stream for the specified channel. Can be used in conjunction with <a>DeleteStreamKey</a> to prevent further streaming to a channel.</p> </li> <li> <p> <a>PutMetadata</a> \u2014 Inserts metadata into the active stream of the specified channel. At most 5 requests per second per channel are allowed, each with a maximum 1 KB payload. (If 5 TPS is not sufficient for your needs, we recommend batching your data into a single PutMetadata call.) At most 155 requests per second per account are allowed.</p> </li> </ul> <p> <b>Stream Key Endpoints</b> </p> <ul> <li> <p> <a>CreateStreamKey</a> \u2014 Creates a stream key, used to initiate a stream, for the specified channel ARN.</p> </li> <li> <p> <a>GetStreamKey</a> \u2014 Gets stream key information for the specified ARN.</p> </li> <li> <p> <a>BatchGetStreamKey</a> \u2014 Performs <a>GetStreamKey</a> on multiple ARNs simultaneously.</p> </li> <li> <p> <a>ListStreamKeys</a> \u2014 Gets summary information about stream keys for the specified channel.</p> </li> <li> <p> <a>DeleteStreamKey</a> \u2014 Deletes the stream key for the specified ARN, so it can no longer be used to stream.</p> </li> </ul> <p> <b>Amazon Web Services Tags Endpoints</b> </p> <ul> <li> <p> <a>TagResource</a> \u2014 Adds or updates tags for the Amazon Web Services resource with the specified ARN.</p> </li> <li> <p> <a>UntagResource</a> \u2014 Removes tags from the resource with the specified ARN.</p> </li> <li> <p> <a>ListTagsForResource</a> \u2014 Gets information about Amazon Web Services tags for the specified ARN.</p> </li> </ul>",
+    "documentation": "<p> <b>Introduction</b> </p> <p>The Amazon Interactive Video Service (IVS) API is REST compatible, using a standard HTTP API and an Amazon Web Services EventBridge event stream for responses. JSON is used for both requests and responses, including errors.</p> <p>The API is an Amazon Web Services regional service. For a list of supported regions and Amazon IVS HTTPS service endpoints, see the <a href=\"https://docs.aws.amazon.com/general/latest/gr/ivs.html\">Amazon IVS page</a> in the <i>Amazon Web Services General Reference</i>.</p> <p> <i> <b>All API request parameters and URLs are case sensitive. </b> </i> </p> <p>For a summary of notable documentation changes in each release, see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/doc-history.html\"> Document History</a>.</p> <p> <b>Allowed Header Values</b> </p> <ul> <li> <p> <code> <b>Accept:</b> </code> application/json</p> </li> <li> <p> <code> <b>Accept-Encoding:</b> </code> gzip, deflate</p> </li> <li> <p> <code> <b>Content-Type:</b> </code>application/json</p> </li> </ul> <p> <b>Resources</b> </p> <p>The following resources contain information about your IVS live stream (see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/getting-started.html\"> Getting Started with Amazon IVS</a>):</p> <ul> <li> <p> <b>Channel</b> \u2014 Stores configuration data related to your live stream. You first create a channel and then use the channel\u2019s stream key to start your live stream. See the Channel endpoints for more information. </p> </li> <li> <p> <b>Stream key</b> \u2014 An identifier assigned by Amazon IVS when you create a channel, which is then used to authorize streaming. See the StreamKey endpoints for more information. <i> <b>Treat the stream key like a secret, since it allows anyone to stream to the channel.</b> </i> </p> </li> <li> <p> <b>Playback key pair</b> \u2014 Video playback may be restricted using playback-authorization tokens, which use public-key encryption. A playback key pair is the public-private pair of keys used to sign and validate the playback-authorization token. See the PlaybackKeyPair endpoints for more information.</p> </li> <li> <p> <b>Recording configuration</b> \u2014 Stores configuration related to recording a live stream and where to store the recorded content. Multiple channels can reference the same recording configuration. See the Recording Configuration endpoints for more information.</p> </li> </ul> <p> <b>Tagging</b> </p> <p>A <i>tag</i> is a metadata label that you assign to an Amazon Web Services resource. A tag comprises a <i>key</i> and a <i>value</i>, both set by you. For example, you might set a tag as <code>topic:nature</code> to label a particular video category. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p> <p>Tags can help you identify and organize your Amazon Web Services resources. For example, you can use the same tag for different resources to indicate that they are related. You can also use tags to manage access (see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_tags.html\"> Access Tags</a>). </p> <p>The Amazon IVS API has these tag-related endpoints: <a>TagResource</a>, <a>UntagResource</a>, and <a>ListTagsForResource</a>. The following resources support tagging: Channels, Stream Keys, Playback Key Pairs, and Recording Configurations.</p> <p>At most 50 tags can be applied to a resource. </p> <p> <b>Authentication versus Authorization</b> </p> <p>Note the differences between these concepts:</p> <ul> <li> <p> <i>Authentication</i> is about verifying identity. You need to be authenticated to sign Amazon IVS API requests.</p> </li> <li> <p> <i>Authorization</i> is about granting permissions. Your IAM roles need to have permissions for Amazon IVS API requests. In addition, authorization is needed to view <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/private-channels.html\">Amazon IVS private channels</a>. (Private channels are channels that are enabled for \"playback authorization.\")</p> </li> </ul> <p> <b>Authentication</b> </p> <p>All Amazon IVS API requests must be authenticated with a signature. The Amazon Web Services Command-Line Interface (CLI) and Amazon IVS Player SDKs take care of signing the underlying API calls for you. However, if your application calls the Amazon IVS API directly, it\u2019s your responsibility to sign the requests.</p> <p>You generate a signature using valid Amazon Web Services credentials that have permission to perform the requested action. For example, you must sign PutMetadata requests with a signature generated from a user account that has the <code>ivs:PutMetadata</code> permission.</p> <p>For more information:</p> <ul> <li> <p>Authentication and generating signatures \u2014 See <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/sig-v4-authenticating-requests.html\">Authenticating Requests (Amazon Web Services Signature Version 4)</a> in the <i>Amazon Web Services General Reference</i>.</p> </li> <li> <p>Managing Amazon IVS permissions \u2014 See <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/security-iam.html\">Identity and Access Management</a> on the Security page of the <i>Amazon IVS User Guide</i>.</p> </li> </ul> <p> <b>Amazon Resource Names (ARNs)</b> </p> <p>ARNs uniquely identify AWS resources. An ARN is required when you need to specify a resource unambiguously across all of AWS, such as in IAM policies and API calls. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\">Amazon Resource Names</a> in the <i>AWS General Reference</i>.</p> <p> <b>Channel Endpoints</b> </p> <ul> <li> <p> <a>CreateChannel</a> \u2014 Creates a new channel and an associated stream key to start streaming.</p> </li> <li> <p> <a>GetChannel</a> \u2014 Gets the channel configuration for the specified channel ARN.</p> </li> <li> <p> <a>BatchGetChannel</a> \u2014 Performs <a>GetChannel</a> on multiple ARNs simultaneously.</p> </li> <li> <p> <a>ListChannels</a> \u2014 Gets summary information about all channels in your account, in the Amazon Web Services region where the API request is processed. This list can be filtered to match a specified name or recording-configuration ARN. Filters are mutually exclusive and cannot be used together. If you try to use both filters, you will get an error (409 Conflict Exception).</p> </li> <li> <p> <a>UpdateChannel</a> \u2014 Updates a channel's configuration. This does not affect an ongoing stream of this channel. You must stop and restart the stream for the changes to take effect.</p> </li> <li> <p> <a>DeleteChannel</a> \u2014 Deletes the specified channel.</p> </li> </ul> <p> <b>StreamKey Endpoints</b> </p> <ul> <li> <p> <a>CreateStreamKey</a> \u2014 Creates a stream key, used to initiate a stream, for the specified channel ARN.</p> </li> <li> <p> <a>GetStreamKey</a> \u2014 Gets stream key information for the specified ARN.</p> </li> <li> <p> <a>BatchGetStreamKey</a> \u2014 Performs <a>GetStreamKey</a> on multiple ARNs simultaneously.</p> </li> <li> <p> <a>ListStreamKeys</a> \u2014 Gets summary information about stream keys for the specified channel.</p> </li> <li> <p> <a>DeleteStreamKey</a> \u2014 Deletes the stream key for the specified ARN, so it can no longer be used to stream.</p> </li> </ul> <p> <b>Stream Endpoints</b> </p> <ul> <li> <p> <a>GetStream</a> \u2014 Gets information about the active (live) stream on a specified channel.</p> </li> <li> <p> <a>GetStreamSession</a> \u2014 Gets metadata on a specified stream.</p> </li> <li> <p> <a>ListStreams</a> \u2014 Gets summary information about live streams in your account, in the Amazon Web Services region where the API request is processed.</p> </li> <li> <p> <a>ListStreamSessions</a> \u2014 Gets a summary of current and previous streams for a specified channel in your account, in the AWS region where the API request is processed.</p> </li> <li> <p> <a>StopStream</a> \u2014 Disconnects the incoming RTMPS stream for the specified channel. Can be used in conjunction with <a>DeleteStreamKey</a> to prevent further streaming to a channel.</p> </li> <li> <p> <a>PutMetadata</a> \u2014 Inserts metadata into the active stream of the specified channel. At most 5 requests per second per channel are allowed, each with a maximum 1 KB payload. (If 5 TPS is not sufficient for your needs, we recommend batching your data into a single PutMetadata call.) At most 155 requests per second per account are allowed.</p> </li> </ul> <p> <b>Private Channel Endpoints</b> </p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/private-channels.html\">Setting Up Private Channels</a> in the <i>Amazon IVS User Guide</i>.</p> <ul> <li> <p> <a>ImportPlaybackKeyPair</a> \u2014 Imports the public portion of a new key pair and returns its <code>arn</code> and <code>fingerprint</code>. The <code>privateKey</code> can then be used to generate viewer authorization tokens, to grant viewers access to private channels (channels enabled for playback authorization).</p> </li> <li> <p> <a>GetPlaybackKeyPair</a> \u2014 Gets a specified playback authorization key pair and returns the <code>arn</code> and <code>fingerprint</code>. The <code>privateKey</code> held by the caller can be used to generate viewer authorization tokens, to grant viewers access to private channels.</p> </li> <li> <p> <a>ListPlaybackKeyPairs</a> \u2014 Gets summary information about playback key pairs.</p> </li> <li> <p> <a>DeletePlaybackKeyPair</a> \u2014 Deletes a specified authorization key pair. This invalidates future viewer tokens generated using the key pair\u2019s <code>privateKey</code>.</p> </li> <li> <p> <a>StartViewerSessionRevocation</a> \u2014 Starts the process of revoking the viewer session associated with a specified channel ARN and viewer ID. Optionally, you can provide a version to revoke viewer sessions less than and including that version.</p> </li> <li> <p> <a>BatchStartViewerSessionRevocation</a> \u2014 Performs <a>StartViewerSessionRevocation</a> on multiple channel ARN and viewer ID pairs simultaneously.</p> </li> </ul> <p> <b>RecordingConfiguration Endpoints</b> </p> <ul> <li> <p> <a>CreateRecordingConfiguration</a> \u2014 Creates a new recording configuration, used to enable recording to Amazon S3.</p> </li> <li> <p> <a>GetRecordingConfiguration</a> \u2014 Gets the recording-configuration metadata for the specified ARN.</p> </li> <li> <p> <a>ListRecordingConfigurations</a> \u2014 Gets summary information about all recording configurations in your account, in the Amazon Web Services region where the API request is processed.</p> </li> <li> <p> <a>DeleteRecordingConfiguration</a> \u2014 Deletes the recording configuration for the specified ARN.</p> </li> </ul> <p> <b>Amazon Web Services Tags Endpoints</b> </p> <ul> <li> <p> <a>TagResource</a> \u2014 Adds or updates tags for the Amazon Web Services resource with the specified ARN.</p> </li> <li> <p> <a>UntagResource</a> \u2014 Removes tags from the resource with the specified ARN.</p> </li> <li> <p> <a>ListTagsForResource</a> \u2014 Gets information about Amazon Web Services tags for the specified ARN.</p> </li> </ul>",
     "metadata": {
         "apiVersion": "2020-07-14",
         "endpointPrefix": "ivs",
         "jsonVersion": "1.1",
         "protocol": "rest-json",
         "serviceAbbreviation": "Amazon IVS",
         "serviceFullName": "Amazon Interactive Video Service",
@@ -100,46 +100,14 @@
                 "shape": "CreateChannelRequest"
             },
             "name": "CreateChannel",
             "output": {
                 "shape": "CreateChannelResponse"
             }
         },
-        "CreatePlaybackRestrictionPolicy": {
-            "documentation": "<p>Creates a new playback restriction policy, for constraining playback by countries and/or origins.</p>",
-            "errors": [
-                {
-                    "shape": "AccessDeniedException"
-                },
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "PendingVerification"
-                },
-                {
-                    "shape": "ThrottlingException"
-                },
-                {
-                    "shape": "ServiceQuotaExceededException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/CreatePlaybackRestrictionPolicy",
-                "responseCode": 200
-            },
-            "input": {
-                "shape": "CreatePlaybackRestrictionPolicyRequest"
-            },
-            "name": "CreatePlaybackRestrictionPolicy",
-            "output": {
-                "shape": "CreatePlaybackRestrictionPolicyResponse"
-            }
-        },
         "CreateRecordingConfiguration": {
             "documentation": "<p>Creates a new recording configuration, used to enable recording to Amazon S3.</p> <p> <b>Known issue:</b> In the us-east-1 region, if you use the Amazon Web Services CLI to create a recording configuration, it returns success even if the S3 bucket is in a different region. In this case, the <code>state</code> of the recording configuration is <code>CREATE_FAILED</code> (instead of <code>ACTIVE</code>). (In other regions, the CLI correctly returns failure if the bucket is in a different region.)</p> <p> <b>Workaround:</b> Ensure that your S3 bucket is in the same region as the recording configuration. If you create a recording configuration in a different region as your S3 bucket, delete that recording configuration and create a new one with an S3 bucket from the correct region.</p>",
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
                 {
@@ -257,43 +225,14 @@
                 "shape": "DeletePlaybackKeyPairRequest"
             },
             "name": "DeletePlaybackKeyPair",
             "output": {
                 "shape": "DeletePlaybackKeyPairResponse"
             }
         },
-        "DeletePlaybackRestrictionPolicy": {
-            "documentation": "<p>Deletes the specified playback restriction policy.</p>",
-            "errors": [
-                {
-                    "shape": "ResourceNotFoundException"
-                },
-                {
-                    "shape": "AccessDeniedException"
-                },
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "PendingVerification"
-                },
-                {
-                    "shape": "ConflictException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/DeletePlaybackRestrictionPolicy",
-                "responseCode": 204
-            },
-            "input": {
-                "shape": "DeletePlaybackRestrictionPolicyRequest"
-            },
-            "name": "DeletePlaybackRestrictionPolicy"
-        },
         "DeleteRecordingConfiguration": {
             "documentation": "<p>Deletes the recording configuration for the specified ARN.</p> <p>If you try to delete a recording configuration that is associated with a channel, you will get an error (409 ConflictException). To avoid this, for all channels that reference the recording configuration, first use <a>UpdateChannel</a> to set the <code>recordingConfigurationArn</code> field to an empty string, then use DeleteRecordingConfiguration.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -393,43 +332,14 @@
                 "shape": "GetPlaybackKeyPairRequest"
             },
             "name": "GetPlaybackKeyPair",
             "output": {
                 "shape": "GetPlaybackKeyPairResponse"
             }
         },
-        "GetPlaybackRestrictionPolicy": {
-            "documentation": "<p>Gets the specified playback restriction policy.</p>",
-            "errors": [
-                {
-                    "shape": "ResourceNotFoundException"
-                },
-                {
-                    "shape": "AccessDeniedException"
-                },
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "PendingVerification"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/GetPlaybackRestrictionPolicy",
-                "responseCode": 200
-            },
-            "input": {
-                "shape": "GetPlaybackRestrictionPolicyRequest"
-            },
-            "name": "GetPlaybackRestrictionPolicy",
-            "output": {
-                "shape": "GetPlaybackRestrictionPolicyResponse"
-            }
-        },
         "GetRecordingConfiguration": {
             "documentation": "<p>Gets the recording configuration for the specified ARN.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -613,43 +523,14 @@
                 "shape": "ListPlaybackKeyPairsRequest"
             },
             "name": "ListPlaybackKeyPairs",
             "output": {
                 "shape": "ListPlaybackKeyPairsResponse"
             }
         },
-        "ListPlaybackRestrictionPolicies": {
-            "documentation": "<p>Gets summary information about playback restriction policies.</p>",
-            "errors": [
-                {
-                    "shape": "AccessDeniedException"
-                },
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "PendingVerification"
-                },
-                {
-                    "shape": "ConflictException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/ListPlaybackRestrictionPolicies",
-                "responseCode": 200
-            },
-            "input": {
-                "shape": "ListPlaybackRestrictionPoliciesRequest"
-            },
-            "name": "ListPlaybackRestrictionPolicies",
-            "output": {
-                "shape": "ListPlaybackRestrictionPoliciesResponse"
-            }
-        },
         "ListRecordingConfigurations": {
             "documentation": "<p>Gets summary information about all recording configurations in your account, in the Amazon Web Services region where the API request is processed.</p>",
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
                 {
@@ -949,46 +830,14 @@
             "input": {
                 "shape": "UpdateChannelRequest"
             },
             "name": "UpdateChannel",
             "output": {
                 "shape": "UpdateChannelResponse"
             }
-        },
-        "UpdatePlaybackRestrictionPolicy": {
-            "documentation": "<p>Updates a specified playback restriction policy.</p>",
-            "errors": [
-                {
-                    "shape": "ResourceNotFoundException"
-                },
-                {
-                    "shape": "AccessDeniedException"
-                },
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "PendingVerification"
-                },
-                {
-                    "shape": "ConflictException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/UpdatePlaybackRestrictionPolicy",
-                "responseCode": 200
-            },
-            "input": {
-                "shape": "UpdatePlaybackRestrictionPolicyRequest"
-            },
-            "name": "UpdatePlaybackRestrictionPolicy",
-            "output": {
-                "shape": "UpdatePlaybackRestrictionPolicyResponse"
-            }
         }
     },
     "shapes": {
         "AccessDeniedException": {
             "documentation": "<p/>",
             "error": {
                 "httpStatusCode": 403,
@@ -1201,41 +1050,33 @@
                     "shape": "IngestEndpoint"
                 },
                 "insecureIngest": {
                     "documentation": "<p>Whether the channel allows insecure RTMP ingest. Default: <code>false</code>.</p>",
                     "shape": "InsecureIngest"
                 },
                 "latencyMode": {
-                    "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers. Default: <code>LOW</code>.</p>",
+                    "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers. Default: <code>LOW</code>. (Note: In the Amazon IVS console, <code>LOW</code> and <code>NORMAL</code> correspond to Ultra-low and Standard, respectively.)</p>",
                     "shape": "ChannelLatencyMode"
                 },
                 "name": {
                     "documentation": "<p>Channel name.</p>",
                     "shape": "ChannelName"
                 },
-                "playbackRestrictionPolicyArn": {
-                    "documentation": "<p>Playback-restriction-policy ARN. A valid ARN value here both specifies the ARN and enables playback restriction. Default: \"\" (empty string, no playback restriction policy is applied).</p>",
-                    "shape": "ChannelPlaybackRestrictionPolicyArn"
-                },
                 "playbackUrl": {
                     "documentation": "<p>Channel playback URL.</p>",
                     "shape": "PlaybackURL"
                 },
                 "preset": {
                     "documentation": "<p>Optional transcode preset for the channel. This is selectable only for <code>ADVANCED_HD</code> and <code>ADVANCED_SD</code> channel types. For those channel types, the default <code>preset</code> is <code>HIGHER_BANDWIDTH_DELIVERY</code>. For other channel types (<code>BASIC</code> and <code>STANDARD</code>), <code>preset</code> is the empty string (<code>\"\"</code>).</p>",
                     "shape": "TranscodePreset"
                 },
                 "recordingConfigurationArn": {
-                    "documentation": "<p>Recording-configuration ARN. A valid ARN value here both specifies the ARN and enables recording. Default: \"\" (empty string, recording is disabled).</p>",
+                    "documentation": "<p>Recording-configuration ARN. A value other than an empty string indicates that recording is enabled. Default: \"\" (empty string, recording is disabled).</p>",
                     "shape": "ChannelRecordingConfigurationArn"
                 },
-                "srt": {
-                    "documentation": "<p>Specifies the endpoint and optional passphrase for streaming with the SRT protocol.</p>",
-                    "shape": "Srt"
-                },
                 "tags": {
                     "documentation": "<p>Tags attached to the resource. Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p>",
                     "shape": "Tags"
                 },
                 "type": {
                     "documentation": "<p>Channel type, which determines the allowable resolution and bitrate. <i>If you exceed the allowable input resolution or bitrate, the stream probably will disconnect immediately.</i> Default: <code>STANDARD</code>. For details, see <a href=\"https://docs.aws.amazon.com/ivs/latest/LowLatencyAPIReference/channel-types.html\">Channel Types</a>.</p>",
                     "shape": "ChannelType"
@@ -1287,20 +1128,14 @@
                 "exceptionMessage": {
                     "documentation": "<p>The stream is offline for the given channel ARN.</p>",
                     "shape": "errorMessage"
                 }
             },
             "type": "structure"
         },
-        "ChannelPlaybackRestrictionPolicyArn": {
-            "max": 128,
-            "min": 0,
-            "pattern": "^$|^arn:aws:ivs:[a-z0-9-]+:[0-9]+:playback-restriction-policy/[a-zA-Z0-9-]+$",
-            "type": "string"
-        },
         "ChannelRecordingConfigurationArn": {
             "max": 128,
             "min": 0,
             "pattern": "^$|^arn:aws:ivs:[a-z0-9-]+:[0-9]+:recording-configuration/[a-zA-Z0-9-]+$",
             "type": "string"
         },
         "ChannelSummary": {
@@ -1315,31 +1150,27 @@
                     "shape": "IsAuthorized"
                 },
                 "insecureIngest": {
                     "documentation": "<p>Whether the channel allows insecure RTMP ingest. Default: <code>false</code>.</p>",
                     "shape": "InsecureIngest"
                 },
                 "latencyMode": {
-                    "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers. Default: <code>LOW</code>.</p>",
+                    "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers. Default: <code>LOW</code>. (Note: In the Amazon IVS console, <code>LOW</code> and <code>NORMAL</code> correspond to Ultra-low and Standard, respectively.)</p>",
                     "shape": "ChannelLatencyMode"
                 },
                 "name": {
                     "documentation": "<p>Channel name.</p>",
                     "shape": "ChannelName"
                 },
-                "playbackRestrictionPolicyArn": {
-                    "documentation": "<p>Playback-restriction-policy ARN. A valid ARN value here both specifies the ARN and enables playback restriction. Default: \"\" (empty string, no playback restriction policy is applied).</p>",
-                    "shape": "ChannelPlaybackRestrictionPolicyArn"
-                },
                 "preset": {
                     "documentation": "<p>Optional transcode preset for the channel. This is selectable only for <code>ADVANCED_HD</code> and <code>ADVANCED_SD</code> channel types. For those channel types, the default <code>preset</code> is <code>HIGHER_BANDWIDTH_DELIVERY</code>. For other channel types (<code>BASIC</code> and <code>STANDARD</code>), <code>preset</code> is the empty string (<code>\"\"</code>).</p>",
                     "shape": "TranscodePreset"
                 },
                 "recordingConfigurationArn": {
-                    "documentation": "<p>Recording-configuration ARN. A valid ARN value here both specifies the ARN and enables recording. Default: \"\" (empty string, recording is disabled).</p>",
+                    "documentation": "<p>Recording-configuration ARN. A value other than an empty string indicates that recording is enabled. Default: \"\" (empty string, recording is disabled).</p>",
                     "shape": "ChannelRecordingConfigurationArn"
                 },
                 "tags": {
                     "documentation": "<p>Tags attached to the resource. Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p>",
                     "shape": "Tags"
                 },
                 "type": {
@@ -1382,35 +1213,31 @@
         "CreateChannelRequest": {
             "members": {
                 "authorized": {
                     "documentation": "<p>Whether the channel is private (enabled for playback authorization). Default: <code>false</code>.</p>",
                     "shape": "Boolean"
                 },
                 "insecureIngest": {
-                    "documentation": "<p>Whether the channel allows insecure RTMP and SRT ingest. Default: <code>false</code>.</p>",
+                    "documentation": "<p>Whether the channel allows insecure RTMP ingest. Default: <code>false</code>.</p>",
                     "shape": "Boolean"
                 },
                 "latencyMode": {
-                    "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers. Default: <code>LOW</code>.</p>",
+                    "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers. (Note: In the Amazon IVS console, <code>LOW</code> and <code>NORMAL</code> correspond to Ultra-low and Standard, respectively.) Default: <code>LOW</code>.</p>",
                     "shape": "ChannelLatencyMode"
                 },
                 "name": {
                     "documentation": "<p>Channel name.</p>",
                     "shape": "ChannelName"
                 },
-                "playbackRestrictionPolicyArn": {
-                    "documentation": "<p>Playback-restriction-policy ARN. A valid ARN value here both specifies the ARN and enables playback restriction. Default: \"\" (empty string, no playback restriction policy is applied).</p>",
-                    "shape": "ChannelPlaybackRestrictionPolicyArn"
-                },
                 "preset": {
                     "documentation": "<p>Optional transcode preset for the channel. This is selectable only for <code>ADVANCED_HD</code> and <code>ADVANCED_SD</code> channel types. For those channel types, the default <code>preset</code> is <code>HIGHER_BANDWIDTH_DELIVERY</code>. For other channel types (<code>BASIC</code> and <code>STANDARD</code>), <code>preset</code> is the empty string (<code>\"\"</code>).</p>",
                     "shape": "TranscodePreset"
                 },
                 "recordingConfigurationArn": {
-                    "documentation": "<p>Recording-configuration ARN. A valid ARN value here both specifies the ARN and enables recording. Default: \"\" (empty string, recording is disabled).</p>",
+                    "documentation": "<p>Recording-configuration ARN. Default: \"\" (empty string, recording is disabled).</p>",
                     "shape": "ChannelRecordingConfigurationArn"
                 },
                 "tags": {
                     "documentation": "<p>Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p>",
                     "shape": "Tags"
                 },
                 "type": {
@@ -1429,48 +1256,14 @@
                 "streamKey": {
                     "documentation": "<p/>",
                     "shape": "StreamKey"
                 }
             },
             "type": "structure"
         },
-        "CreatePlaybackRestrictionPolicyRequest": {
-            "members": {
-                "allowedCountries": {
-                    "documentation": "<p>A list of country codes that control geoblocking restriction. Allowed values are the officially assigned <a href=\"https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2\">ISO 3166-1 alpha-2</a> codes. Default: All countries (an empty array).</p>",
-                    "shape": "PlaybackRestrictionPolicyAllowedCountryList"
-                },
-                "allowedOrigins": {
-                    "documentation": "<p>A list of origin sites that control CORS restriction. Allowed values are the same as valid values of the Origin header defined at <a href=\"https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Origin\">https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Origin</a>. Default: All origins (an empty array).</p>",
-                    "shape": "PlaybackRestrictionPolicyAllowedOriginList"
-                },
-                "enableStrictOriginEnforcement": {
-                    "documentation": "<p>Whether channel playback is constrained by origin site. Default: <code>false</code>.</p>",
-                    "shape": "PlaybackRestrictionPolicyEnableStrictOriginEnforcement"
-                },
-                "name": {
-                    "documentation": "<p>Playback-restriction-policy name. The value does not need to be unique.</p>",
-                    "shape": "PlaybackRestrictionPolicyName"
-                },
-                "tags": {
-                    "documentation": "<p>Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p>",
-                    "shape": "Tags"
-                }
-            },
-            "type": "structure"
-        },
-        "CreatePlaybackRestrictionPolicyResponse": {
-            "members": {
-                "playbackRestrictionPolicy": {
-                    "documentation": "<p/>",
-                    "shape": "PlaybackRestrictionPolicy"
-                }
-            },
-            "type": "structure"
-        },
         "CreateRecordingConfigurationRequest": {
             "members": {
                 "destinationConfiguration": {
                     "documentation": "<p>A complex type that contains a destination configuration for where recorded video will be stored.</p>",
                     "shape": "DestinationConfiguration"
                 },
                 "name": {
@@ -1557,26 +1350,14 @@
             ],
             "type": "structure"
         },
         "DeletePlaybackKeyPairResponse": {
             "members": {},
             "type": "structure"
         },
-        "DeletePlaybackRestrictionPolicyRequest": {
-            "members": {
-                "arn": {
-                    "documentation": "<p>ARN of the playback restriction policy to be deleted.</p>",
-                    "shape": "PlaybackRestrictionPolicyArn"
-                }
-            },
-            "required": [
-                "arn"
-            ],
-            "type": "structure"
-        },
         "DeleteRecordingConfigurationRequest": {
             "members": {
                 "arn": {
                     "documentation": "<p>ARN of the recording configuration to be deleted.</p>",
                     "shape": "RecordingConfigurationArn"
                 }
             },
@@ -1645,35 +1426,14 @@
                 "keyPair": {
                     "documentation": "<zonbook></zonbook><xhtml></xhtml>",
                     "shape": "PlaybackKeyPair"
                 }
             },
             "type": "structure"
         },
-        "GetPlaybackRestrictionPolicyRequest": {
-            "members": {
-                "arn": {
-                    "documentation": "<p>ARN of the playback restriction policy to be returned.</p>",
-                    "shape": "PlaybackRestrictionPolicyArn"
-                }
-            },
-            "required": [
-                "arn"
-            ],
-            "type": "structure"
-        },
-        "GetPlaybackRestrictionPolicyResponse": {
-            "members": {
-                "playbackRestrictionPolicy": {
-                    "documentation": "<p/>",
-                    "shape": "PlaybackRestrictionPolicy"
-                }
-            },
-            "type": "structure"
-        },
         "GetRecordingConfigurationRequest": {
             "members": {
                 "arn": {
                     "documentation": "<p>ARN of the recording configuration to be retrieved.</p>",
                     "shape": "RecordingConfigurationArn"
                 }
             },
@@ -1830,18 +1590,14 @@
         },
         "ListChannelsRequest": {
             "members": {
                 "filterByName": {
                     "documentation": "<p>Filters the channel list to match the specified name.</p>",
                     "shape": "ChannelName"
                 },
-                "filterByPlaybackRestrictionPolicyArn": {
-                    "documentation": "<p>Filters the channel list to match the specified policy.</p>",
-                    "shape": "ChannelPlaybackRestrictionPolicyArn"
-                },
                 "filterByRecordingConfigurationArn": {
                     "documentation": "<p>Filters the channel list to match the specified recording-configuration ARN.</p>",
                     "shape": "ChannelRecordingConfigurationArn"
                 },
                 "maxResults": {
                     "documentation": "<p>Maximum number of channels to return. Default: 100.</p>",
                     "shape": "MaxChannelResults"
@@ -1894,43 +1650,14 @@
                 }
             },
             "required": [
                 "keyPairs"
             ],
             "type": "structure"
         },
-        "ListPlaybackRestrictionPoliciesRequest": {
-            "members": {
-                "maxResults": {
-                    "documentation": "<p>Maximum number of policies to return. Default: 1.</p>",
-                    "shape": "MaxPlaybackRestrictionPolicyResults"
-                },
-                "nextToken": {
-                    "documentation": "<p>The first policy to retrieve. This is used for pagination; see the <code>nextToken</code> response field.</p>",
-                    "shape": "PaginationToken"
-                }
-            },
-            "type": "structure"
-        },
-        "ListPlaybackRestrictionPoliciesResponse": {
-            "members": {
-                "nextToken": {
-                    "documentation": "<p>If there are more channels than <code>maxResults</code>, use <code>nextToken</code> in the request to get the next set.</p>",
-                    "shape": "PaginationToken"
-                },
-                "playbackRestrictionPolicies": {
-                    "documentation": "<p>List of the matching policies.</p>",
-                    "shape": "PlaybackRestrictionPolicyList"
-                }
-            },
-            "required": [
-                "playbackRestrictionPolicies"
-            ],
-            "type": "structure"
-        },
         "ListRecordingConfigurationsRequest": {
             "members": {
                 "maxResults": {
                     "documentation": "<p>Maximum number of recording configurations to return. Default: your service quota or 100, whichever is smaller. </p>",
                     "shape": "MaxRecordingConfigurationResults"
                 },
                 "nextToken": {
@@ -2095,20 +1822,14 @@
         },
         "MaxPlaybackKeyPairResults": {
             "box": true,
             "max": 100,
             "min": 1,
             "type": "integer"
         },
-        "MaxPlaybackRestrictionPolicyResults": {
-            "box": true,
-            "max": 100,
-            "min": 1,
-            "type": "integer"
-        },
         "MaxRecordingConfigurationResults": {
             "box": true,
             "max": 100,
             "min": 1,
             "type": "integer"
         },
         "MaxStreamKeyResults": {
@@ -2204,128 +1925,14 @@
                 }
             },
             "type": "structure"
         },
         "PlaybackPublicKeyMaterial": {
             "type": "string"
         },
-        "PlaybackRestrictionPolicy": {
-            "documentation": "<p>An object representing a policy to constrain playback by country and/or origin sites.</p>",
-            "members": {
-                "allowedCountries": {
-                    "documentation": "<p>A list of country codes that control geoblocking restriction. Allowed values are the officially assigned <a href=\"https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2\">ISO 3166-1 alpha-2</a> codes. Default: All countries (an empty array).</p>",
-                    "shape": "PlaybackRestrictionPolicyAllowedCountryList"
-                },
-                "allowedOrigins": {
-                    "documentation": "<p>A list of origin sites that control CORS restriction. Allowed values are the same as valid values of the Origin header defined at <a href=\"https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Origin\">https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Origin</a>. Default: All origins (an empty array).</p>",
-                    "shape": "PlaybackRestrictionPolicyAllowedOriginList"
-                },
-                "arn": {
-                    "documentation": "<p>Playback-restriction-policy ARN</p>",
-                    "shape": "PlaybackRestrictionPolicyArn"
-                },
-                "enableStrictOriginEnforcement": {
-                    "documentation": "<p>Whether channel playback is constrained by origin site. Default: <code>false</code>.</p>",
-                    "shape": "PlaybackRestrictionPolicyEnableStrictOriginEnforcement"
-                },
-                "name": {
-                    "documentation": "<p>Playback-restriction-policy name. The value does not need to be unique.</p>",
-                    "shape": "PlaybackRestrictionPolicyName"
-                },
-                "tags": {
-                    "documentation": "<p>Tags attached to the resource. Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p>",
-                    "shape": "Tags"
-                }
-            },
-            "required": [
-                "allowedCountries",
-                "allowedOrigins",
-                "arn"
-            ],
-            "type": "structure"
-        },
-        "PlaybackRestrictionPolicyAllowedCountry": {
-            "max": 2,
-            "min": 2,
-            "type": "string"
-        },
-        "PlaybackRestrictionPolicyAllowedCountryList": {
-            "member": {
-                "shape": "PlaybackRestrictionPolicyAllowedCountry"
-            },
-            "type": "list"
-        },
-        "PlaybackRestrictionPolicyAllowedOrigin": {
-            "max": 128,
-            "min": 0,
-            "type": "string"
-        },
-        "PlaybackRestrictionPolicyAllowedOriginList": {
-            "member": {
-                "shape": "PlaybackRestrictionPolicyAllowedOrigin"
-            },
-            "type": "list"
-        },
-        "PlaybackRestrictionPolicyArn": {
-            "max": 128,
-            "min": 1,
-            "pattern": "^arn:aws:ivs:[a-z0-9-]+:[0-9]+:playback-restriction-policy/[a-zA-Z0-9-]+$",
-            "type": "string"
-        },
-        "PlaybackRestrictionPolicyEnableStrictOriginEnforcement": {
-            "box": true,
-            "type": "boolean"
-        },
-        "PlaybackRestrictionPolicyList": {
-            "member": {
-                "shape": "PlaybackRestrictionPolicySummary"
-            },
-            "type": "list"
-        },
-        "PlaybackRestrictionPolicyName": {
-            "max": 128,
-            "min": 0,
-            "pattern": "^[a-zA-Z0-9-_]*$",
-            "type": "string"
-        },
-        "PlaybackRestrictionPolicySummary": {
-            "documentation": "<p>Summary information about a PlaybackRestrictionPolicy.</p>",
-            "members": {
-                "allowedCountries": {
-                    "documentation": "<p>A list of country codes that control geoblocking restriction. Allowed values are the officially assigned <a href=\"https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2\">ISO 3166-1 alpha-2</a> codes. Default: All countries (an empty array).</p>",
-                    "shape": "PlaybackRestrictionPolicyAllowedCountryList"
-                },
-                "allowedOrigins": {
-                    "documentation": "<p>A list of origin sites that control CORS restriction. Allowed values are the same as valid values of the Origin header defined at <a href=\"https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Origin\">https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Origin</a>. Default: All origins (an empty array).</p>",
-                    "shape": "PlaybackRestrictionPolicyAllowedOriginList"
-                },
-                "arn": {
-                    "documentation": "<p>Playback-restriction-policy ARN</p>",
-                    "shape": "PlaybackRestrictionPolicyArn"
-                },
-                "enableStrictOriginEnforcement": {
-                    "documentation": "<p>Whether channel playback is constrained by origin site. Default: <code>false</code>.</p>",
-                    "shape": "PlaybackRestrictionPolicyEnableStrictOriginEnforcement"
-                },
-                "name": {
-                    "documentation": "<p>Playback-restriction-policy name. The value does not need to be unique.</p>",
-                    "shape": "PlaybackRestrictionPolicyName"
-                },
-                "tags": {
-                    "documentation": "<p>Tags attached to the resource. Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p>",
-                    "shape": "Tags"
-                }
-            },
-            "required": [
-                "allowedCountries",
-                "allowedOrigins",
-                "arn"
-            ],
-            "type": "structure"
-        },
         "PlaybackURL": {
             "type": "string"
         },
         "PutMetadataRequest": {
             "members": {
                 "channelArn": {
                     "documentation": "<p>ARN of the channel into which metadata is inserted. This channel must have an active stream.</p>",
@@ -2542,35 +2149,14 @@
                 "exceptionMessage": {
                     "documentation": "<p>Request would cause a service quota to be exceeded.</p>",
                     "shape": "errorMessage"
                 }
             },
             "type": "structure"
         },
-        "Srt": {
-            "documentation": "<p>Specifies information needed to stream using the SRT protocol.</p>",
-            "members": {
-                "endpoint": {
-                    "documentation": "<p>The endpoint to be used when streaming with IVS using the SRT protocol.</p>",
-                    "shape": "SrtEndpoint"
-                },
-                "passphrase": {
-                    "documentation": "<p>Auto-generated passphrase to enable encryption. This field is applicable only if the end user has <i>not</i> enabled the <code>insecureIngest</code> option for the channel.</p>",
-                    "shape": "SrtPassphrase"
-                }
-            },
-            "type": "structure"
-        },
-        "SrtEndpoint": {
-            "type": "string"
-        },
-        "SrtPassphrase": {
-            "sensitive": true,
-            "type": "string"
-        },
         "StartViewerSessionRevocationRequest": {
             "members": {
                 "channelArn": {
                     "documentation": "<p>The ARN of the channel associated with the viewer session to revoke.</p>",
                     "shape": "ChannelArn"
                 },
                 "viewerId": {
@@ -3030,15 +2616,15 @@
                 "resourceArn": {
                     "documentation": "<p>ARN of the resource for which tags are to be removed. The ARN must be URL-encoded.</p>",
                     "location": "uri",
                     "locationName": "resourceArn",
                     "shape": "ResourceArn"
                 },
                 "tagKeys": {
-                    "documentation": "<p>Array of tags to be removed. Array of maps, each of the form <code>string:string (key:value)</code>. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p>",
+                    "documentation": "<p>Array of tags to be removed. Array of maps, each of the form s<code>tring:string (key:value)</code>. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p>",
                     "location": "querystring",
                     "locationName": "tagKeys",
                     "shape": "TagKeyList"
                 }
             },
             "required": [
                 "resourceArn",
@@ -3057,35 +2643,31 @@
                     "shape": "ChannelArn"
                 },
                 "authorized": {
                     "documentation": "<p>Whether the channel is private (enabled for playback authorization).</p>",
                     "shape": "Boolean"
                 },
                 "insecureIngest": {
-                    "documentation": "<p>Whether the channel allows insecure RTMP and SRT ingest. Default: <code>false</code>.</p>",
+                    "documentation": "<p>Whether the channel allows insecure RTMP ingest. Default: <code>false</code>.</p>",
                     "shape": "Boolean"
                 },
                 "latencyMode": {
-                    "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers.</p>",
+                    "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers. (Note: In the Amazon IVS console, <code>LOW</code> and <code>NORMAL</code> correspond to Ultra-low and Standard, respectively.)</p>",
                     "shape": "ChannelLatencyMode"
                 },
                 "name": {
                     "documentation": "<p>Channel name.</p>",
                     "shape": "ChannelName"
                 },
-                "playbackRestrictionPolicyArn": {
-                    "documentation": "<p>Playback-restriction-policy ARN. A valid ARN value here both specifies the ARN and enables playback restriction. If this is set to an empty string, playback restriction policy is disabled.</p>",
-                    "shape": "ChannelPlaybackRestrictionPolicyArn"
-                },
                 "preset": {
                     "documentation": "<p>Optional transcode preset for the channel. This is selectable only for <code>ADVANCED_HD</code> and <code>ADVANCED_SD</code> channel types. For those channel types, the default <code>preset</code> is <code>HIGHER_BANDWIDTH_DELIVERY</code>. For other channel types (<code>BASIC</code> and <code>STANDARD</code>), <code>preset</code> is the empty string (<code>\"\"</code>).</p>",
                     "shape": "TranscodePreset"
                 },
                 "recordingConfigurationArn": {
-                    "documentation": "<p>Recording-configuration ARN. A valid ARN value here both specifies the ARN and enables recording. If this is set to an empty string, recording is disabled.</p>",
+                    "documentation": "<p>Recording-configuration ARN. If this is set to an empty string, recording is disabled. A value other than an empty string indicates that recording is enabled</p>",
                     "shape": "ChannelRecordingConfigurationArn"
                 },
                 "type": {
                     "documentation": "<p>Channel type, which determines the allowable resolution and bitrate. <i>If you exceed the allowable input resolution or bitrate, the stream probably will disconnect immediately.</i> Default: <code>STANDARD</code>. For details, see <a href=\"https://docs.aws.amazon.com/ivs/latest/LowLatencyAPIReference/channel-types.html\">Channel Types</a>.</p>",
                     "shape": "ChannelType"
                 }
             },
@@ -3093,57 +2675,19 @@
                 "arn"
             ],
             "type": "structure"
         },
         "UpdateChannelResponse": {
             "members": {
                 "channel": {
-                    "documentation": "<p>Object specifying the updated channel.</p>",
                     "shape": "Channel"
                 }
             },
             "type": "structure"
         },
-        "UpdatePlaybackRestrictionPolicyRequest": {
-            "members": {
-                "allowedCountries": {
-                    "documentation": "<p>A list of country codes that control geoblocking restriction. Allowed values are the officially assigned <a href=\"https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2\">ISO 3166-1 alpha-2</a> codes. Default: All countries (an empty array).</p>",
-                    "shape": "PlaybackRestrictionPolicyAllowedCountryList"
-                },
-                "allowedOrigins": {
-                    "documentation": "<p>A list of origin sites that control CORS restriction. Allowed values are the same as valid values of the Origin header defined at <a href=\"https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Origin\">https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Origin</a>. Default: All origins (an empty array).</p>",
-                    "shape": "PlaybackRestrictionPolicyAllowedOriginList"
-                },
-                "arn": {
-                    "documentation": "<p>ARN of the playback-restriction-policy to be updated.</p>",
-                    "shape": "PlaybackRestrictionPolicyArn"
-                },
-                "enableStrictOriginEnforcement": {
-                    "documentation": "<p>Whether channel playback is constrained by origin site. Default: <code>false</code>.</p>",
-                    "shape": "PlaybackRestrictionPolicyEnableStrictOriginEnforcement"
-                },
-                "name": {
-                    "documentation": "<p>Playback-restriction-policy name. The value does not need to be unique.</p>",
-                    "shape": "PlaybackRestrictionPolicyName"
-                }
-            },
-            "required": [
-                "arn"
-            ],
-            "type": "structure"
-        },
-        "UpdatePlaybackRestrictionPolicyResponse": {
-            "members": {
-                "playbackRestrictionPolicy": {
-                    "documentation": "<p>Object specifying the updated policy.</p>",
-                    "shape": "PlaybackRestrictionPolicy"
-                }
-            },
-            "type": "structure"
-        },
         "ValidationException": {
             "documentation": "<p/>",
             "error": {
                 "httpStatusCode": 400,
                 "senderFault": true
             },
             "exception": true,
```

### Comparing `botocore-a-la-carte-ivs-1.34.82/botocore_a_la_carte_ivs.egg-info/PKG-INFO` & `botocore-a-la-carte-ivs-1.34.9/botocore_a_la_carte_ivs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ivs
-Version: 1.34.82
+Version: 1.34.9
 Summary: ivs data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ivs-1.34.82/setup.py` & `botocore-a-la-carte-ivs-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ivs',
-    version="1.34.82",
+    version="1.34.9",
     description='ivs data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ivs/*/*.json'],
```

