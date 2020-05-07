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
|Authorization|Bearer {token}. Required.|

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
      "id": "79517a47-7a47-7951-477a-5179477a5179",
      "creationDateTime": "String (timestamp)",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)",
      "completionDateTime": "String (timestamp)",
      "error": {
        "@odata.type": "microsoft.graph.classificationError"
      },
      "datastoreId": "String",
      "uploadAgentId": "String",
      "fields": [
        "String"
      ],
      "fileName": "String",
      "checksum": "String",
      "dataUploadURI": "String",
      "remainingBlockCount": "Integer",
      "totalBlockCount": "Integer",
      "state": "String",
      "uploadCompletionDateTime": "String (timestamp)",
      "processingCompletionDateTime": "String (timestamp)",
      "rowsPerBlock": "Integer",
      "totalJobCount": "Integer",
      "remainingJobCount": "Integer",
      "salt": "String"
    }
  ]
}
```

