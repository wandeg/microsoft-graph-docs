---
title: "List exactMatchUploadAgents"
description: "Get the exactMatchUploadAgents from the exactMatchUploadAgents navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List exactMatchUploadAgents

Namespace: microsoft.graph

Get the exactMatchUploadAgents from the exactMatchUploadAgents navigation property.

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
GET /dataClassification/exactMatchUploadAgents
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
If successful, this method returns a `200 OK` response code and a collection of [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_exactmatchuploadagent"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/exactMatchUploadAgents
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.exactmatchuploadagent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.exactMatchUploadAgent",
      "id": "211b34ad-34ad-211b-ad34-1b21ad341b21",
      "description": "Description value",
      "creationDateTime": "2016-12-31T23:59:05.697798+03:00"
    }
  ]
}
```

