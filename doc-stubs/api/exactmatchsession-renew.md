---
title: "exactMatchSession: renew"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# renew

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}/renew
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this action returns a `200 OK` response code and a [exactMatchSession](../resources/exactmatchsession.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "exactmatchsession_renew"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}/renew
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactmatchsession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.exactMatchSession",
    "id": "String (identifier)",
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
}
```

