---
title: "List persons"
description: "List properties and relationships of the person objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List persons

Namespace: microsoft.graph

List properties and relationships of the [person](../resources/person.md) objects.

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
GET /me/people
GET /users/{usersId}/people
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_person"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/people
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.person)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2438

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.person",
      "id": "28bbef2d-ef2d-28bb-2def-bb282defbb28",
      "displayName": "Display Name value",
      "givenName": "Given Name value",
      "surname": "Surname value",
      "birthday": "Birthday value",
      "personNotes": "Person Notes value",
      "isFavorite": true,
      "emailAddresses": [
        {
          "@odata.type": "microsoft.graph.rankedEmailAddress",
          "address": "Address value",
          "rank": "Double"
        }
      ],
      "phones": [
        {
          "@odata.type": "microsoft.graph.phone",
          "type": "String",
          "number": "Number value"
        }
      ],
      "postalAddresses": [
        {
          "@odata.type": "microsoft.graph.location",
          "locationEmailAddress": "Location Email Address value",
          "address": {
            "@odata.type": "microsoft.graph.physicalAddress",
            "type": "String",
            "postOfficeBox": "Post Office Box value",
            "street": "Street value",
            "city": "City value",
            "state": "State value",
            "countryOrRegion": "Country Or Region value",
            "postalCode": "Postal Code value"
          },
          "coordinates": {
            "@odata.type": "microsoft.graph.outlookGeoCoordinates",
            "altitude": "Double",
            "latitude": "Double",
            "longitude": "Double",
            "accuracy": "Double",
            "altitudeAccuracy": "Double"
          },
          "locationUri": "Location Uri value",
          "locationType": "String",
          "uniqueId": "Unique Id value",
          "uniqueIdType": "String"
        }
      ],
      "websites": [
        {
          "@odata.type": "microsoft.graph.website",
          "type": "String"
        }
      ],
      "title": "Title value",
      "companyName": "Company Name value",
      "yomiCompany": "Yomi Company value",
      "department": "Department value",
      "officeLocation": "Office Location value",
      "profession": "Profession value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.personDataSource",
          "type": "Type value"
        }
      ],
      "mailboxType": "Mailbox Type value",
      "personType": "Person Type value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```

