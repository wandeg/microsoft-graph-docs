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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [cartToClassAssociation](../resources/carttoclassassociation.md) object.

The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/carttoclassassociation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|deviceCartIds|String collection|**TODO: Add Description**|
|classroomIds|String collection|**TODO: Add Description**|



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
Content-length: 228

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "version": "Integer",
  "displayName": "String",
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "classroomIds": [
    "String"
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
  "id": "9171852e-852e-9171-2e85-71912e857191",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": "Integer",
  "displayName": "String",
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "classroomIds": [
    "String"
  ]
}
```

