---
title: "Add sessions"
description: "Add sessions by posting to the sessions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add sessions

Namespace: microsoft.graph

Add sessions by posting to the sessions collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
|salt|String||



## Response
If successful, this method returns a `201 Created` response code and a [exactMatchSession](../resources/exactmatchsession.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_exactmatchsession_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions
Content-type: application/json
Content-length: 1388

{
  "@odata.type": "#microsoft.graph.exactMatchSession",
  "creationDateTime": "2017-01-01T00:02:38.3339201+00:00",
  "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
  "lastUpdatedDateTime": "2016-12-31T23:58:15.2250773+00:00",
  "completionDateTime": "2016-12-31T23:58:05.4513555+00:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2017-01-01T00:02:25.6061378+00:00",
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
  "uploadCompletionDateTime": "2017-01-01T00:02:05.8475063+00:00",
  "processingCompletionDateTime": "2017-01-01T00:01:57.0595644+00:00",
  "rowsPerBlock": 12,
  "totalJobCount": 13,
  "remainingJobCount": 1,
  "salt": "Salt value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactmatchsession"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1437

{
  "@odata.type": "#microsoft.graph.exactMatchSession",
  "id": "b84d3f36-3f36-b84d-363f-4db8363f4db8",
  "creationDateTime": "2017-01-01T00:02:38.3339201+00:00",
  "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
  "lastUpdatedDateTime": "2016-12-31T23:58:15.2250773+00:00",
  "completionDateTime": "2016-12-31T23:58:05.4513555+00:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2017-01-01T00:02:25.6061378+00:00",
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
  "uploadCompletionDateTime": "2017-01-01T00:02:05.8475063+00:00",
  "processingCompletionDateTime": "2017-01-01T00:01:57.0595644+00:00",
  "rowsPerBlock": 12,
  "totalJobCount": 13,
  "remainingJobCount": 1,
  "salt": "Salt value"
}
```

