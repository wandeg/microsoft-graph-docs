---
title: "Create cartToClassAssociation"
description: "Create a new cartToClassAssociation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create cartToClassAssociation

Namespace: microsoft.graph

Create a new [cartToClassAssociation](../resources/carttoclassassociation.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/carttoclassassociation.md) object.

The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/carttoclassassociation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|version|Int32|Version of the CartToClassAssociation.|
|displayName|String|Admin provided name of the device configuration.|
|description|String|Admin provided description of the CartToClassAssociation.|
|deviceCartIds|String collection|Identifiers of device carts to be associated with classes.|
|classroomIds|String collection|Identifiers of classrooms to be associated with device carts.|



## Response
If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/carttoclassassociation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_carttoclassassociation_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/cartToClassAssociations
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.carttoclassassociation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 442

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "f4785119-5119-f478-1951-78f4195178f4",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
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

