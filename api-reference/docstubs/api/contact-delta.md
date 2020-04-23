---
title: "contact: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /me/contacts/delta
GET /users/{usersId}/contacts/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [contact](../resources/contact.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/contacts/delta
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.contact)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.contact",
      "id": "7c888695-8695-7c88-9586-887c9586887c",
      "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
      "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
      "changeKey": "Change Key value",
      "categories": [
        "Categories value"
      ],
      "parentFolderId": "Parent Folder Id value",
      "birthday": "2017-01-01T00:01:20.6670608+03:00",
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
          "@odata.type": "microsoft.graph.emailAddress"
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
      "businessHomePage": "Business Home Page value",
      "assistantName": "Assistant Name value",
      "manager": "Manager value",
      "homePhones": [
        "Home Phones value"
      ],
      "mobilePhone": "Mobile Phone value",
      "businessPhones": [
        "Business Phones value"
      ],
      "homeAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "businessAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "otherAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "spouseName": "Spouse Name value",
      "personalNotes": "Personal Notes value",
      "children": [
        "Children value"
      ]
    }
  ]
}
```

