---
title: "Update exactMatchSession"
description: "Update the properties of a exactMatchSession object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update exactMatchSession

Namespace: microsoft.graph

Update the properties of a [exactMatchSession](../resources/exactmatchsession.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [exactMatchSession](../resources/exactmatchsession.md) object.

The following table shows the properties that are required when you create the [exactMatchSession](../resources/exactmatchsession.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|creationDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|startDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|lastUpdatedDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|completionDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|error|[classificationError](../resources/classificationerror.md)| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|datastoreId|String||
|uploadAgentId|String||
|fields|String collection||
|fileName|String||
|checksum|String||
|dataUploadURI|String||
|remainingBlockCount|Int32||
|totalBlockCount|Int32||
|state|String||
|uploadCompletionDateTime|DateTimeOffset||
|processingCompletionDateTime|DateTimeOffset||
|rowsPerBlock|Int32||
|totalJobCount|Int32||
|remainingJobCount|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [exactMatchSession](../resources/exactmatchsession.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_exactmatchsession"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}
Content-type: application/json
Content-length: 1363

{
  "@odata.type": "#microsoft.graph.exactMatchSession",
  "creationDateTime": "2017-01-01T00:02:11.4839005+03:00",
  "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
  "lastUpdatedDateTime": "2016-12-31T23:57:46.2985547+03:00",
  "completionDateTime": "2016-12-31T23:56:58.8026209+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:59:22.9712113+03:00",
      "clientRequestId": "Client Request Id value",
      "activityId": "Activity Id value"
    },
    "details": [
      {
        "@odata.type": "microsoft.graph.classifcationErrorBase"
      }
    ]
  },
  "datastoreId": "Datastore Id value",
  "uploadAgentId": "Upload Agent Id value",
  "fields": [
    "Fields value"
  ],
  "fileName": "File Name value",
  "checksum": "Checksum value",
  "dataUploadURI": "Data Upload URI value",
  "remainingBlockCount": 3,
  "totalBlockCount": 15,
  "state": "State value",
  "uploadCompletionDateTime": "2016-12-31T23:59:20.8844305+03:00",
  "processingCompletionDateTime": "2017-01-01T00:02:46.9156622+03:00",
  "rowsPerBlock": 12,
  "totalJobCount": 13,
  "remainingJobCount": 1
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1412

{
  "@odata.type": "#microsoft.graph.exactMatchSession",
  "id": "8a727218-7218-8a72-1872-728a1872728a",
  "creationDateTime": "2017-01-01T00:02:11.4839005+03:00",
  "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
  "lastUpdatedDateTime": "2016-12-31T23:57:46.2985547+03:00",
  "completionDateTime": "2016-12-31T23:56:58.8026209+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:59:22.9712113+03:00",
      "clientRequestId": "Client Request Id value",
      "activityId": "Activity Id value"
    },
    "details": [
      {
        "@odata.type": "microsoft.graph.classifcationErrorBase"
      }
    ]
  },
  "datastoreId": "Datastore Id value",
  "uploadAgentId": "Upload Agent Id value",
  "fields": [
    "Fields value"
  ],
  "fileName": "File Name value",
  "checksum": "Checksum value",
  "dataUploadURI": "Data Upload URI value",
  "remainingBlockCount": 3,
  "totalBlockCount": 15,
  "state": "State value",
  "uploadCompletionDateTime": "2016-12-31T23:59:20.8844305+03:00",
  "processingCompletionDateTime": "2017-01-01T00:02:46.9156622+03:00",
  "rowsPerBlock": 12,
  "totalJobCount": 13,
  "remainingJobCount": 1
}
```

