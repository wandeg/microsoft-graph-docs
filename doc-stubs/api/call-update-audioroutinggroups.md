---
title: "Update audioRoutingGroups"
description: "Update the properties of an audioRoutingGroups object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update audioRoutingGroups

Namespace: microsoft.graph

Update the properties of an audioRoutingGroups object.

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
PATCH /app/calls/{callId}/audioRoutingGroups
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [audioRoutingGroup](../resources/audioroutinggroup.md) object.

The following table shows the properties that are required when you create the [audioRoutingGroup](../resources/audioroutinggroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|routingMode|routingMode|**TODO: Add Description**. Possible values are: `oneToOne`, `multicast`.|
|sources|String collection|**TODO: Add Description**|
|receivers|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_audioroutinggroups"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/app/calls/{callId}/audioRoutingGroups
Content-Type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.audioRoutingGroup",
  "routingMode": "String",
  "sources": [
    "String"
  ],
  "receivers": [
    "String"
  ]
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
  "@odata.type": "#microsoft.graph.audioRoutingGroup",
  "id": "cbd1e0c9-e0c9-cbd1-c9e0-d1cbc9e0d1cb",
  "routingMode": "String",
  "sources": [
    "String"
  ],
  "receivers": [
    "String"
  ]
}
```

