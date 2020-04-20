---
title: "Create people"
description: "Create a new people object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create people

Namespace: microsoft.graph

Create a new people object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/people
POST /users/{usersId}/people
POST /invitations/{invitationsId}/invitedUser/people
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [person](../resources/person.md) object.

The following table shows the properties that are required when you create the [person](../resources/person.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|birthday|String|**TODO: Add Description**|
|personNotes|String|**TODO: Add Description**|
|isFavorite|Boolean|**TODO: Add Description**|
|emailAddresses|[rankedEmailAddress](../resources/rankedemailaddress.md) collection|**TODO: Add Description**|
|phones|[phone](../resources/phone.md) collection|**TODO: Add Description**|
|postalAddresses|[location](../resources/location.md) collection|**TODO: Add Description**|
|websites|[website](../resources/website.md) collection|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|yomiCompany|String|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|profession|String|**TODO: Add Description**|
|sources|[personDataSource](../resources/persondatasource.md) collection|**TODO: Add Description**|
|mailboxType|String|**TODO: Add Description**|
|personType|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [person](../resources/person.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_person_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/people
Content-Type: application/json
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.person",
  "id": "70aa66c0-66c0-70aa-c066-aa70c066aa70",
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

