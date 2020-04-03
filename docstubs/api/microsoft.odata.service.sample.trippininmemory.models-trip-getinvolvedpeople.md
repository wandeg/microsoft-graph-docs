---
title: "getInvolvedPeople"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getInvolvedPeople

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



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
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "trip_getinvolvedpeople"
}
-->
``` http

```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.odata.service.sample.trippininmemory.models.person)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 733

{
  "value": [
    {
      "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.person",
      "userName": "User Name value",
      "firstName": "First Name value",
      "lastName": "Last Name value",
      "middleName": "Middle Name value",
      "gender": "String",
      "age": 3,
      "emails": [
        "Emails value"
      ],
      "addressInfo": [
        {
          "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.location"
        }
      ],
      "homeAddress": {
        "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.location"
      },
      "favoriteFeature": "String",
      "features": [
        "String"
      ]
    }
  ]
}
```

