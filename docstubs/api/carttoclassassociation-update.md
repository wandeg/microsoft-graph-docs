---
title: "Update cartToClassAssociation"
description: "Update the properties of a cartToClassAssociation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update cartToClassAssociation

Namespace: microsoft.graph

Update the properties of a [cartToClassAssociation](../resources/carttoclassassociation.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/carttoclassassociation.md) object.

The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/carttoclassassociation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|version|Int32||
|displayName|String||
|description|String||
|deviceCartIds|String collection||
|classroomIds|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/carttoclassassociation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_carttoclassassociation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "ea0718a5-18a5-ea07-a518-07eaa51807ea",
  "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00",
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

