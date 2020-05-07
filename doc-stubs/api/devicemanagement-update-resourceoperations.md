---
title: "Update resourceOperations"
description: "Update the properties of a resourceOperations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update resourceOperations

Namespace: microsoft.graph

Update the properties of a resourceOperations object.

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
PATCH /deviceManagement/resourceOperations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [resourceOperation](../resources/resourceoperation.md) object.

The following table shows the properties that are required when you create the [resourceOperation](../resources/resourceoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resource|String|**TODO: Add Description**|
|resourceName|String|**TODO: Add Description**|
|actionName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|enabledForScopeValidation|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/resourceoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_resourceoperations"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceOperations
Content-Type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resource": "String",
  "resourceName": "String",
  "actionName": "String",
  "description": "String",
  "enabledForScopeValidation": "Boolean"
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
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "c3880c11-0c11-c388-110c-88c3110c88c3",
  "resource": "String",
  "resourceName": "String",
  "actionName": "String",
  "description": "String",
  "enabledForScopeValidation": "Boolean"
}
```

