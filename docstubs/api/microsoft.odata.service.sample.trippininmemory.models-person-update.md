---
title: "Update Person"
description: "Update the properties of a Person object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update Person

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Update the properties of a [Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.

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
PATCH /Me
PATCH /People/{PeopleId}
PATCH /NewComePeople/{NewComePeopleId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.

The following table shows the properties that are required when you create the [Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md).

|Property|Type|Description|
|:---|:---|:---|
|UserName|String||
|FirstName|String||
|LastName|String||
|MiddleName|String||
|Gender|Enumeration| Possible values are: `Male`, `Female`, `Unknow`.|
|Age|Int64||
|Emails|String collection||
|AddressInfo|[Location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md) collection||
|HomeAddress|[Location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md)||
|FavoriteFeature|Enumeration| Possible values are: `Feature1`, `Feature2`, `Feature3`, `Feature4`.|
|Features|Enumeration collection| Possible values are: `Feature1`, `Feature2`, `Feature3`, `Feature4`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_person"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Me
Content-type: application/json
Content-length: 875

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Person",
  "UserName": "User Name value",
  "FirstName": "First Name value",
  "LastName": "Last Name value",
  "MiddleName": "Middle Name value",
  "Gender": "String",
  "Age": 3,
  "Emails": [
    "Emails value"
  ],
  "AddressInfo": [
    {
      "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Location",
      "Address": "Address value",
      "City": {
        "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.City",
        "Name": "Name value",
        "CountryRegion": "Country Region value",
        "Region": "Region value"
      }
    }
  ],
  "HomeAddress": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Location"
  },
  "FavoriteFeature": "String",
  "Features": [
    "String"
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
Content-Length: 875

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Person",
  "UserName": "User Name value",
  "FirstName": "First Name value",
  "LastName": "Last Name value",
  "MiddleName": "Middle Name value",
  "Gender": "String",
  "Age": 3,
  "Emails": [
    "Emails value"
  ],
  "AddressInfo": [
    {
      "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Location",
      "Address": "Address value",
      "City": {
        "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.City",
        "Name": "Name value",
        "CountryRegion": "Country Region value",
        "Region": "Region value"
      }
    }
  ],
  "HomeAddress": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Location"
  },
  "FavoriteFeature": "String",
  "Features": [
    "String"
  ]
}
```

