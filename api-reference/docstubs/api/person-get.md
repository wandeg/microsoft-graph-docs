---
title: "Get person"
description: "Read the properties and relationships of a person object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get person

Namespace: microsoft.graph

Read the properties and relationships of a [person](../resources/person.md) object.

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
GET /me/people/{personId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_person"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/people/{personId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.person",
    "id": "a4232f52-2f52-a423-522f-23a4522f23a4",
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
}
```

