---
title: "List Friends"
description: "Get the Persons from the Friends navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List Friends

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Get the Persons from the Friends navigation property.

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
GET /Me/Friends
GET /People/{PeopleId}/Friends
GET /NewComePeople/{NewComePeopleId}/Friends
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
If successful, this method returns a `200 OK` response code and a collection of [Person](../resources/person.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_person"
}
-->
``` http
GET https://graph.microsoft.com/beta/Me/Friends
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
Content-Length: 1024

{
  "value": [
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
  ]
}
```

