---
title: "Create connectorGroups"
description: "Create a new connectorGroups object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create connectorGroups

Namespace: microsoft.graph

Create a new connectorGroups object.

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
POST ** Collection URI for microsoft.graph.connectorGroup not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [connectorGroup](../resources/connectorgroup.md) object.

The following table shows the properties that are required when you create the [connectorGroup](../resources/connectorgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|connectorGroupType|connectorGroupType|**TODO: Add Description**. Possible values are: `applicationProxy`.|
|isDefault|Boolean|**TODO: Add Description**|
|region|connectorGroupRegion|**TODO: Add Description**. Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`, `unknownFutureValue`.|



## Response

If successful, this method returns a `201 Created` response code and a [connectorGroup](../resources/connectorgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connectorgroups"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.connectorGroup not found
Content-Type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.connectorGroup",
  "name": "String",
  "connectorGroupType": "String",
  "isDefault": "Boolean",
  "region": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorgroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.connectorGroup",
  "id": "475bef30-ef30-475b-30ef-5b4730ef5b47",
  "name": "String",
  "connectorGroupType": "String",
  "isDefault": "Boolean",
  "region": "String"
}
```

