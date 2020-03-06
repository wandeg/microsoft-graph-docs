---
title: "Get cartToClassAssociation"
description: "Read properties and relationships of the cartToClassAssociation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get cartToClassAssociation

Namespace: microsoft.graph

Read properties and relationships of the [cartToClassAssociation](../resources/carttoclassassociation.md) object.

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
GET /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [cartToClassAssociation](../resources/carttoclassassociation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_carttoclassassociation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cartToClassAssociation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 488

{
  "value": {
    "@odata.type": "#microsoft.graph.cartToClassAssociation",
    "id": "20f1cc2f-cc2f-20f1-2fcc-f1202fccf120",
    "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
    "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
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
}
```

