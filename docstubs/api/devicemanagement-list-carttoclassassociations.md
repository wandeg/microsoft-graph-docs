---
title: "List cartToClassAssociations"
description: "Get the cartToClassAssociations from the cartToClassAssociations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List cartToClassAssociations

Namespace: microsoft.graph

Get the cartToClassAssociations from the cartToClassAssociations navigation property.

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
GET /deviceManagement/cartToClassAssociations
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [cartToClassAssociation](../resources/carttoclassassociation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_carttoclassassociation"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.carttoclassassociation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 528

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cartToClassAssociation",
      "id": "1f1e8089-8089-1f1e-8980-1e1f89801e1f",
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
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
  ]
}
```

