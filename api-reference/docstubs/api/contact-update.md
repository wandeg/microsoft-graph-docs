---
title: "Update contact"
description: "Update the properties of a contact object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update contact

Namespace: microsoft.graph

Update the properties of a [contact](../resources/contact.md) object.

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
PATCH /me/contacts/{contactId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
  "name": "update_contact"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/contacts/{contactId}
Content-Type: application/json
Content-length: 1903

{
  "@odata.type": "#microsoft.graph.contact",
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
      "@odata.type": "microsoft.graph.emailAddress",
      "name": "Name value",
      "address": "Address value"
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
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
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
      "@odata.type": "microsoft.graph.emailAddress",
      "name": "Name value",
      "address": "Address value"
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
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
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
```

