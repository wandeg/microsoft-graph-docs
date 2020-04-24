---
title: "Update exactMatchSession"
description: "Update the properties of an exactMatchSession object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update exactMatchSession

Namespace: microsoft.graph

Update the properties of an [exactMatchSession](../resources/exactmatchsession.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [exactMatchSession](../resources/exactmatchsession.md) object.

The following table shows the properties that are required when you create the [exactMatchSession](../resources/exactmatchsession.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|creationDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|startDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|completionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|error|[classificationError](../resources/classificationerror.md)|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|datastoreId|String|**TODO: Add Description**|
|uploadAgentId|String|**TODO: Add Description**|
|fields|String collection|**TODO: Add Description**|
|fileName|String|**TODO: Add Description**|
|checksum|String|**TODO: Add Description**|
|dataUploadURI|String|**TODO: Add Description**|
|remainingBlockCount|Int32|**TODO: Add Description**|
|totalBlockCount|Int32|**TODO: Add Description**|
|state|String|**TODO: Add Description**|
|uploadCompletionDateTime|DateTimeOffset|**TODO: Add Description**|
|processingCompletionDateTime|DateTimeOffset|**TODO: Add Description**|
|rowsPerBlock|Int32|**TODO: Add Description**|
|totalJobCount|Int32|**TODO: Add Description**|
|remainingJobCount|Int32|**TODO: Add Description**|
|salt|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [exactMatchSession](../resources/exactmatchsession.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_exactmatchsession"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}
Content-Type: application/json
Content-length: 1387

{
  "@odata.type": "#microsoft.graph.exactMatchSession",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "lastUpdatedDateTime": "2016-12-31T23:58:57.2159356+03:00",
  "completionDateTime": "2016-12-31T23:58:01.1668342+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:57:05.4991702+03:00",
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
  "uploadCompletionDateTime": "2017-01-01T00:01:11.5771327+03:00",
  "processingCompletionDateTime": "2017-01-01T00:02:36.4990361+03:00",
  "rowsPerBlock": 12,
  "totalJobCount": 13,
  "remainingJobCount": 1,
  "salt": "Salt value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.exactMatchSession",
  "id": "8dad370f-370f-8dad-0f37-ad8d0f37ad8d",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "lastUpdatedDateTime": "2016-12-31T23:58:57.2159356+03:00",
  "completionDateTime": "2016-12-31T23:58:01.1668342+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:57:05.4991702+03:00",
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
  "uploadCompletionDateTime": "2017-01-01T00:01:11.5771327+03:00",
  "processingCompletionDateTime": "2017-01-01T00:02:36.4990361+03:00",
  "rowsPerBlock": 12,
  "totalJobCount": 13,
  "remainingJobCount": 1,
  "salt": "Salt value"
}
```

