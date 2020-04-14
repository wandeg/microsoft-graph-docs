---
title: "Create friends"
description: "Create friends by posting to the friends collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create friends

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Create friends by posting to the friends collection.

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
POST /me/friends/$ref
POST /people/{peopleId}/friends/$ref
POST /newComePeople/{newComePeopleId}/friends/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_person_from_people"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/friends
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
  "truncated": true,
  "@odata.type": "microsoft.odata.service.sample.trippininmemory.models.person"
}
-->
``` http
HTTP/1.1 201 Created
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

