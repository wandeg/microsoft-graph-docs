---
title: "Get exactMatchSession"
description: "Read properties and relationships of the exactMatchSession object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get exactMatchSession

Namespace: microsoft.graph

Read properties and relationships of the [exactMatchSession](../resources/exactmatchsession.md) object.

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
GET /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [exactMatchSession](../resources/exactmatchsession.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_exactmatchsession"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactMatchSession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1507

{
  "value": {
    "@odata.type": "#microsoft.graph.exactMatchSession",
    "id": "61c0268e-268e-61c0-8e26-c0618e26c061",
    "creationDateTime": "2016-12-31T23:57:41.730992+00:00",
    "startDateTime": "2016-12-31T23:58:12.4547779+00:00",
    "lastUpdatedDateTime": "2017-01-01T00:01:50.447451+00:00",
    "completionDateTime": "2017-01-01T00:03:33.3771518+00:00",
    "error": {
      "@odata.type": "microsoft.graph.classificationError",
      "code": "Code value",
      "message": "Message value",
      "target": "Target value",
      "innerError": {
        "@odata.type": "microsoft.graph.classificationInnerError",
        "errorDateTime": "2017-01-01T00:00:20.7240967+00:00",
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
    "uploadCompletionDateTime": "2016-12-31T23:57:26.0021489+00:00",
    "processingCompletionDateTime": "2016-12-31T23:57:11.1336438+00:00",
    "rowsPerBlock": 12,
    "totalJobCount": 13,
    "remainingJobCount": 1
  }
}
```

