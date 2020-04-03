---
title: "Get contact"
description: "Read properties and relationships of the contact object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get contact

Namespace: microsoft.graph

Read properties and relationships of the [contact](../resources/contact.md) object.

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
GET /me/contacts/{contactId}
GET /users/{usersId}/contacts/{contactId}
GET /me/contactFolders/{contactFolderId}/contacts/{contactId}
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
If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_contact"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/contacts/{contactId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2862

{
  "value": {
    "@odata.type": "#microsoft.graph.contact",
    "id": "41c9f783-f783-41c9-83f7-c94183f7c941",
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "parentFolderId": "Parent Folder Id value",
    "birthday": "2016-12-31T23:56:58.1718665+00:00",
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

