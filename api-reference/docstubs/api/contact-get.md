---
title: "Get contact"
description: "Read properties and relationships of a contact object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get contact

Namespace: microsoft.graph

Read properties and relationships of a [contact](../resources/contact.md) object.

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
GET /me/contacts/{contactId}
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
If successful, this method returns a `200 OK` response code and a [contact](../resources/contact.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_contact"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/contacts/{contactId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.contact",
    "id": "379f1904-1904-379f-0419-9f3704199f37",
    "createdDateTime": "2016-12-31T23:57:35.7108579+03:00",
    "lastModifiedDateTime": "2016-12-31T23:58:38.9820934+03:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "parentFolderId": "Parent Folder Id value",
    "birthday": "2017-01-01T00:00:47.3962323+03:00",
    "fileAs": "File As value",
    "displayName": "Display Name value",
    "givenName": "Given Name value",
    "initials": "Initials value",
    "middleName": "Middle Name value",
    "nickName": "Nick Name value",
    "surname": "Surname value",
    "title": "Title value",
    "yomiGivenName": "Yomi Given Name value",
    "yomiSurname": "Yomi Surname value",
    "yomiCompanyName": "Yomi Company Name value",
    "generation": "Generation value",
    "emailAddresses": [
      {
        "@odata.type": "microsoft.graph.typedEmailAddress",
        "name": "Name value",
        "address": "Address value",
        "type": "String",
        "otherLabel": "Other Label value"
      }
    ],
    "websites": [
      {
        "@odata.type": "microsoft.graph.website",
        "type": "String"
      }
    ],
    "imAddresses": [
      "Im Addresses value"
    ],
    "jobTitle": "Job Title value",
    "companyName": "Company Name value",
    "department": "Department value",
    "officeLocation": "Office Location value",
    "profession": "Profession value",
    "assistantName": "Assistant Name value",
    "manager": "Manager value",
    "phones": [
      {
        "@odata.type": "microsoft.graph.phone",
        "type": "String",
        "number": "Number value"
      }
    ],
    "postalAddresses": [
      {
        "@odata.type": "microsoft.graph.physicalAddress",
        "type": "String",
        "postOfficeBox": "Post Office Box value",
        "street": "Street value",
        "city": "City value",
        "state": "State value",
        "countryOrRegion": "Country Or Region value",
        "postalCode": "Postal Code value"
      }
    ],
    "spouseName": "Spouse Name value",
    "personalNotes": "Personal Notes value",
    "children": [
      "Children value"
    ],
    "weddingAnniversary": "Date",
    "gender": "Gender value",
    "isFavorite": true,
    "flag": {
      "@odata.type": "microsoft.graph.followupFlag",
      "completedDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone",
        "dateTime": "Date Time value",
        "timeZone": "Time Zone value"
      },
      "dueDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "startDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "flagStatus": "String"
    }
  }
}
```

