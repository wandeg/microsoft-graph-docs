---
title: "Update people"
description: "Update the properties of a people object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update people

Namespace: microsoft.graph

Update the properties of a people object.

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
PATCH /me/people
PATCH /users/{usersId}/people
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

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
|scoredEmailAddresses|[scoredEmailAddress](../resources/scoredemailaddress.md) collection|**TODO: Add Description**|
|phones|[phone](../resources/phone.md) collection|**TODO: Add Description**|
|postalAddresses|[location](../resources/location.md) collection|**TODO: Add Description**|
|websites|[website](../resources/website.md) collection|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|yomiCompany|String|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|profession|String|**TODO: Add Description**|
|personType|[personType](../resources/persontype.md)|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|imAddress|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [person](../resources/person.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_people"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/people
Content-Type: application/json
Content-length: 2135

{
  "@odata.type": "#microsoft.graph.person",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "surname": "Surname value",
  "birthday": "Birthday value",
  "personNotes": "Person Notes value",
  "isFavorite": true,
  "scoredEmailAddresses": [
    {
      "@odata.type": "microsoft.graph.scoredEmailAddress",
      "address": "Address value",
      "relevanceScore": "Double",
      "selectionLikelihood": "String",
      "itemId": "Item Id value"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone",
      "type": "String",
      "number": "Number value",
      "region": "Region value",
      "language": "Language value"
    }
  ],
  "postalAddresses": [
    {
      "@odata.type": "microsoft.graph.location",
      "locationEmailAddress": "Location Email Address value",
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress",
        "street": "Street value",
        "city": "City value",
        "state": "State value",
        "countryOrRegion": "Country Or Region value",
        "postalCode": "Postal Code value"
      },
      "locationUri": "Location Uri value",
      "coordinates": {
        "@odata.type": "microsoft.graph.outlookGeoCoordinates",
        "latitude": "Double",
        "longitude": "Double",
        "accuracy": "Double",
        "altitude": "Double",
        "altitudeAccuracy": "Double"
      },
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
  "jobTitle": "Job Title value",
  "companyName": "Company Name value",
  "yomiCompany": "Yomi Company value",
  "department": "Department value",
  "officeLocation": "Office Location value",
  "profession": "Profession value",
  "personType": {
    "@odata.type": "microsoft.graph.personType",
    "class": "Class value",
    "subclass": "Subclass value"
  },
  "userPrincipalName": "User Principal Name value",
  "imAddress": "Im Address value"
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
{
  "@odata.type": "#microsoft.graph.person",
  "id": "451ae651-e651-451a-51e6-1a4551e61a45",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "surname": "Surname value",
  "birthday": "Birthday value",
  "personNotes": "Person Notes value",
  "isFavorite": true,
  "scoredEmailAddresses": [
    {
      "@odata.type": "microsoft.graph.scoredEmailAddress",
      "address": "Address value",
      "relevanceScore": "Double",
      "selectionLikelihood": "String",
      "itemId": "Item Id value"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone",
      "type": "String",
      "number": "Number value",
      "region": "Region value",
      "language": "Language value"
    }
  ],
  "postalAddresses": [
    {
      "@odata.type": "microsoft.graph.location",
      "locationEmailAddress": "Location Email Address value",
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress",
        "street": "Street value",
        "city": "City value",
        "state": "State value",
        "countryOrRegion": "Country Or Region value",
        "postalCode": "Postal Code value"
      },
      "locationUri": "Location Uri value",
      "coordinates": {
        "@odata.type": "microsoft.graph.outlookGeoCoordinates",
        "latitude": "Double",
        "longitude": "Double",
        "accuracy": "Double",
        "altitude": "Double",
        "altitudeAccuracy": "Double"
      },
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
  "jobTitle": "Job Title value",
  "companyName": "Company Name value",
  "yomiCompany": "Yomi Company value",
  "department": "Department value",
  "officeLocation": "Office Location value",
  "profession": "Profession value",
  "personType": {
    "@odata.type": "microsoft.graph.personType",
    "class": "Class value",
    "subclass": "Subclass value"
  },
  "userPrincipalName": "User Principal Name value",
  "imAddress": "Im Address value"
}
```

