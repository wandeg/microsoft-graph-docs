---
title: "Get exactMatchUploadAgent"
description: "Read properties and relationships of the exactMatchUploadAgent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get exactMatchUploadAgent

Namespace: microsoft.graph

Read properties and relationships of the [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.

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
GET /dataClassification/exactMatchUploadAgents/{exactMatchUploadAgentId}
GET /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}/uploadAgent
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
If successful, this method returns a `200 OK` response code and [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_exactmatchuploadagent"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/exactMatchUploadAgents/{exactMatchUploadAgentId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactMatchUploadAgent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "value": {
    "@odata.type": "#microsoft.graph.exactMatchUploadAgent",
    "id": "2fa71cf3-1cf3-2fa7-f31c-a72ff31ca72f",
    "description": "Description value",
    "creationDateTime": "2016-12-31T23:57:41.730992+00:00"
  }
}
```

