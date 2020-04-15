---
title: "Update person"
description: "Update the properties of a person object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update person

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Update the properties of a [person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.

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
PATCH /me
PATCH /people/{peopleId}
PATCH /newComePeople/{newComePeopleId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.

The following table shows the properties that are required when you create the [person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md).

|Property|Type|Description|
|:---|:---|:---|
|userName|String|This is the primary key|
|firstName|String||
|lastName|String||
|middleName|String||
|gender|Enumeration| Possible values are: `male`, `female`, `unknow`.|
|age|Int64||
|emails|String collection||
|addresses|[location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md) collection||
|homeAddress|[location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md)||
|favoriteFeature|Enumeration| Possible values are: `feature1`, `feature2`, `feature3`, `feature4`.|
|features|Enumeration collection| Possible values are: `feature1`, `feature2`, `feature3`, `feature4`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_person"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me
Content-type: application/json
Content-length: 873

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
  "addresses": [
    {
      "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.location",
      "address": "Address value",
      "city": {
        "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.city",
        "name": "Name value",
        "countryRegion": "Country Region value",
        "region": "Region value"
      }
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 873

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
  "addresses": [
    {
      "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.location",
      "address": "Address value",
      "city": {
        "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.city",
        "name": "Name value",
        "countryRegion": "Country Region value",
        "region": "Region value"
      }
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
```

