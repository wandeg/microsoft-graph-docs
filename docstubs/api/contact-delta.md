---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph



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
GET /me/contacts/delta
GET /users/{usersId}/contacts/delta
GET /me/contactFolders/{contactFolderId}/contacts/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [contact](../resources/contact.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/contacts/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.contact)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2100

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.contact",
      "id": "e2d3407f-407f-e2d3-7f40-d3e27f40d3e2",
      "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
      "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
      "changeKey": "Change Key value",
      "categories": [
        "Categories value"
      ],
      "parentFolderId": "Parent Folder Id value",
      "birthday": "2016-12-31T23:58:50.7295567+00:00",
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
          "@odata.type": "microsoft.graph.typedEmailAddress"
        }
      ],
      "websites": [
        {
          "@odata.type": "microsoft.graph.website"
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
          "@odata.type": "microsoft.graph.phone"
        }
      ],
      "postalAddresses": [
        {
          "@odata.type": "microsoft.graph.physicalAddress"
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
        "@odata.type": "microsoft.graph.followupFlag"
      }
    }
  ]
}
```

