---
title: "Update exactMatchUploadAgent"
description: "Update the properties of a exactMatchUploadAgent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update exactMatchUploadAgent

Update the properties of a [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.

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
PATCH /dataClassification/exactMatchUploadAgents/{exactMatchUploadAgentId}
PATCH /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}/uploadAgent
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [exactMatchUploadAgent](../resources/exactMatchUploadAgent.md) object.

The following table shows the properties that are required when you create the [exactMatchUploadAgent](../resources/exactmatchuploadagent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String||
|creationDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_exactmatchuploadagent"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/dataClassification/exactMatchUploadAgents/{exactMatchUploadAgentId}
Content-type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.exactMatchUploadAgent",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:59.0982804+03:00"
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
  "id": "2b200352-0352-2b20-5203-202b5203202b",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:59.0982804+03:00"
}
```

