---
title: "Create cartToClassAssociations"
description: "Create a new cartToClassAssociations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create cartToClassAssociations

Namespace: microsoft.graph

Create a new cartToClassAssociations object.

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
POST /deviceManagement/cartToClassAssociations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [cartToClassAssociation](../resources/carttoclassassociation.md) object.

The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/carttoclassassociation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|version|Int32|Version of the CartToClassAssociation.|
|displayName|String|Admin provided name of the device configuration.|
|description|String|Admin provided description of the CartToClassAssociation.|
|deviceCartIds|String collection|Identifiers of device carts to be associated with classes.|
|classroomIds|String collection|Identifiers of classrooms to be associated with device carts.|



## Response
If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/carttoclassassociation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_carttoclassassociation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-Type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.carttoclassassociation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "7ee4e426-e426-7ee4-26e4-e47e26e4e47e",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

