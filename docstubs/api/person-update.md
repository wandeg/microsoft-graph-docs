---
title: "Update person"
description: "Update the properties of a person object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update person

Namespace: microsoft.graph

Update the properties of a [person](../resources/person.md) object.

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
PATCH /me/people/{personId}
PATCH /users/{usersId}/people/{personId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [person](../resources/person.md) object.

The following table shows the properties that are required when you create the [person](../resources/person.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|givenName|String||
|surname|String||
|birthday|String||
|personNotes|String||
|isFavorite|Boolean||
|emailAddresses|[rankedEmailAddress](../resources/rankedemailaddress.md) collection||
|phones|[phone](../resources/phone.md) collection||
|postalAddresses|[location](../resources/location.md) collection||
|websites|[website](../resources/website.md) collection||
|title|String||
|companyName|String||
|yomiCompany|String||
|department|String||
|officeLocation|String||
|profession|String||
|sources|[personDataSource](../resources/persondatasource.md) collection||
|mailboxType|String||
|personType|String||
|userPrincipalName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [person](../resources/person.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_person"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/people/{personId}
Content-type: application/json
Content-length: 2072

{
  "@odata.type": "#microsoft.graph.person",
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
Content-Length: 2121

{
  "@odata.type": "#microsoft.graph.person",
  "id": "be4ffae2-fae2-be4f-e2fa-4fbee2fa4fbe",
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
```

