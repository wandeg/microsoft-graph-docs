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
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [resourceOperation](../resources/resourceoperation.md) object.

The following table shows the properties that are required when you create the [resourceOperation](../resources/resourceoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resourceName|String|Name of the Resource this operation is performed on.|
|actionName|String|Type of action this operation is going to perform. The actionName should be concise and limited to as few words as possible.|
|description|String|Description of the resource operation. The description is used in mouse-over text for the operation when shown in the Azure Portal.|



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
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
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
  "id": "f06b9cc5-9cc5-f06b-c59c-6bf0c59c6bf0",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

