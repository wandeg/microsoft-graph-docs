---
title: "Add members"
description: "Add members by posting to the members collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add members

Namespace: microsoft.graph

Add members by posting to the members collection.

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
POST ** Collection URI for microsoft.graph.connector not found/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [connector](../resources/connector.md) object.

The following table shows the properties that are required when you create the [connector](../resources/connector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|machineName|String|**TODO: Add Description**|
|externalIp|String|**TODO: Add Description**|
|status|connectorStatus|**TODO: Add Description**. Possible values are: `active`, `inactive`.|



## Response

If successful, this method returns a `204 No Content` response code and a [connector](../resources/connector.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectors"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.connector not found/$ref
Content-Type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.connector",
  "machineName": "String",
  "externalIp": "String",
  "status": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.connector",
  "id": "7aa5aca1-aca1-7aa5-a1ac-a57aa1aca57a",
  "machineName": "String",
  "externalIp": "String",
  "status": "String"
}
```

