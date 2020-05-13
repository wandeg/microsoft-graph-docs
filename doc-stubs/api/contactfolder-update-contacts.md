---
title: "Update contacts"
description: "Update the properties of a contacts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update contacts

Namespace: microsoft.graph

Update the properties of a contacts object.

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
PATCH /users/{usersId}/contactFolders/{contactFolderId}/contacts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [contact](../resources/contact.md) object.

The following table shows the properties that are required when you create the [contact](../resources/contact.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|categories|String collection|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|parentFolderId|String|**TODO: Add Description**|
|birthday|DateTimeOffset|**TODO: Add Description**|
|fileAs|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|initials|String|**TODO: Add Description**|
|middleName|String|**TODO: Add Description**|
|nickName|String|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|yomiGivenName|String|**TODO: Add Description**|
|yomiSurname|String|**TODO: Add Description**|
|yomiCompanyName|String|**TODO: Add Description**|
|generation|String|**TODO: Add Description**|
|emailAddresses|[emailAddress](../resources/emailaddress.md) collection|**TODO: Add Description**|
|imAddresses|String collection|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|profession|String|**TODO: Add Description**|
|businessHomePage|String|**TODO: Add Description**|
|assistantName|String|**TODO: Add Description**|
|manager|String|**TODO: Add Description**|
|homePhones|String collection|**TODO: Add Description**|
|mobilePhone|String|**TODO: Add Description**|
|businessPhones|String collection|**TODO: Add Description**|
|homeAddress|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|businessAddress|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|otherAddress|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|spouseName|String|**TODO: Add Description**|
|personalNotes|String|**TODO: Add Description**|
|children|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_contacts"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/contactFolders/{contactFolderId}/contacts
Content-Type: application/json
Content-length: 1309

{
  "@odata.type": "#microsoft.graph.contact",
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
      "@odata.type": "microsoft.graph.emailAddress"
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
  "businessHomePage": "String",
  "assistantName": "String",
  "manager": "String",
  "homePhones": [
    "String"
  ],
  "mobilePhone": "String",
  "businessPhones": [
    "String"
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
  "spouseName": "String",
  "personalNotes": "String",
  "children": [
    "String"
  ]
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.contact",
  "id": "3162acd5-acd5-3162-d5ac-6231d5ac6231",
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
      "@odata.type": "microsoft.graph.emailAddress"
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
  "businessHomePage": "String",
  "assistantName": "String",
  "manager": "String",
  "homePhones": [
    "String"
  ],
  "mobilePhone": "String",
  "businessPhones": [
    "String"
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
  "spouseName": "String",
  "personalNotes": "String",
  "children": [
    "String"
  ]
}
```

