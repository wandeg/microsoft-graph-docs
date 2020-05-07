---
title: "Update parent"
description: "Update the properties of a parent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update parent

Namespace: microsoft.graph

Update the properties of a parent object.

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
PATCH ** Collection URI for microsoft.graph.governanceResource not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [governanceResource](../resources/governanceresource.md) object.

The following table shows the properties that are required when you create the [governanceResource](../resources/governanceresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|externalId|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|registeredDateTime|DateTimeOffset|**TODO: Add Description**|
|registeredRoot|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [governanceResource](../resources/governanceresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_parent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta** Collection URI for microsoft.graph.governanceResource not found
Content-Type: application/json
Content-length: 237

{
  "@odata.type": "#microsoft.graph.governanceResource",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String"
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
  "@odata.type": "#microsoft.graph.governanceResource",
  "id": "29cde8df-e8df-29cd-dfe8-cd29dfe8cd29",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String"
}
```

