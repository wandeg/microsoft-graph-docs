---
title: "List sessions"
description: "Get the exactMatchSessions from the sessions navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List sessions

Namespace: microsoft.graph

Get the exactMatchSessions from the sessions navigation property.

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
GET /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [exactMatchSession](../resources/exactmatchsession.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_exactmatchsession"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.exactmatchsession)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

