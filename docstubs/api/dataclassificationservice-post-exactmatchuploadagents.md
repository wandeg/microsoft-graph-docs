---
title: "Add exactMatchUploadAgents"
description: "Add exactMatchUploadAgents by posting to the exactMatchUploadAgents collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add exactMatchUploadAgents

Namespace: microsoft.graph

Add exactMatchUploadAgents by posting to the exactMatchUploadAgents collection.

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
POST /dataClassification/exactMatchUploadAgents/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.

The following table shows the properties that are required when you create the [exactMatchUploadAgent](../resources/exactmatchuploadagent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String||
|creationDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_exactmatchuploadagent_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/exactMatchUploadAgents
Content-type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.exactMatchUploadAgent",
  "description": "Description value",
  "creationDateTime": "2016-12-31T23:57:30.6368517+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactmatchuploadagent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 211

{
  "@odata.type": "#microsoft.graph.exactMatchUploadAgent",
  "id": "723f02ee-02ee-723f-ee02-3f72ee023f72",
  "description": "Description value",
  "creationDateTime": "2016-12-31T23:57:30.6368517+03:00"
}
```

