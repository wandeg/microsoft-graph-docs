---
title: "Update exactMatchUploadAgent"
description: "Update the properties of a exactMatchUploadAgent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update exactMatchUploadAgent

Namespace: microsoft.graph

Update the properties of a [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.

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
PATCH /dataClassification/exactMatchUploadAgents/{exactMatchUploadAgentId}
PATCH /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}/uploadAgent
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.

The following table shows the properties that are required when you create the [exactMatchUploadAgent](../resources/exactmatchuploadagent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String||
|creationDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_exactmatchuploadagent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/exactMatchUploadAgents/{exactMatchUploadAgentId}
Content-type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.exactMatchUploadAgent",
  "description": "Description value",
  "creationDateTime": "2016-12-31T23:56:46.0826945+03:00"
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
Content-Length: 211

{
  "@odata.type": "#microsoft.graph.exactMatchUploadAgent",
  "id": "134ec828-c828-134e-28c8-4e1328c84e13",
  "description": "Description value",
  "creationDateTime": "2016-12-31T23:56:46.0826945+03:00"
}
```

