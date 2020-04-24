---
title: "Create audioRoutingGroups"
description: "Create a new audioRoutingGroups object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create audioRoutingGroups

Namespace: microsoft.graph

Create a new audioRoutingGroups object.

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
POST /communications/calls/{callId}/audioRoutingGroups
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_audioroutinggroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/communications/calls/{callId}/audioRoutingGroups
Content-Type: application/json
Content-length: 177

{
  "@odata.type": "#microsoft.graph.audioRoutingGroup",
  "routingMode": "String",
  "sources": [
    "Sources value"
  ],
  "receivers": [
    "Receivers value"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioroutinggroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.audioRoutingGroup",
  "id": "75df7ad9-7ad9-75df-d97a-df75d97adf75",
  "routingMode": "String",
  "sources": [
    "Sources value"
  ],
  "receivers": [
    "Receivers value"
  ]
}
```

