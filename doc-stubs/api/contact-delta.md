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
|Authorization|Bearer {token}. Required.|

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
      "id": "String (identifier)",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "changeKey": "String",
      "categories": [
        "String"
      ],
      "parentFolderId": "String",
      "birthday": "String (timestamp)",
      "fileAs": "String",
      "displayName": "String",
      "givenName": "String",
      "initials": "String",
      "middleName": "String",
      "nickName": "String",
      "surname": "String",
      "title": "String",
      "yomiGivenName": "String",
      "yomiSurname": "String",
      "yomiCompanyName": "String",
      "generation": "String",
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
        "String"
      ],
      "jobTitle": "String",
      "companyName": "String",
      "department": "String",
      "officeLocation": "String",
      "profession": "String",
      "assistantName": "String",
      "manager": "String",
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
      "spouseName": "String",
      "personalNotes": "String",
      "children": [
        "String"
      ],
      "weddingAnniversary": "Date",
      "gender": "String",
      "isFavorite": "Boolean",
      "flag": {
        "@odata.type": "microsoft.graph.followupFlag"
      }
    }
  ]
}
```

