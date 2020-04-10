---
title: "Add contacts"
description: "Add contacts by posting to the contacts collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add contacts

Namespace: microsoft.graph

Add contacts by posting to the contacts collection.

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
POST /me/contacts/$ref
POST /users/{usersId}/contacts/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [contact](../resources/contact.md) object.

The following table shows the properties that are required when you create the [contact](../resources/contact.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|parentFolderId|String||
|birthday|DateTimeOffset||
|fileAs|String||
|displayName|String||
|givenName|String||
|initials|String||
|middleName|String||
|nickName|String||
|surname|String||
|title|String||
|yomiGivenName|String||
|yomiSurname|String||
|yomiCompanyName|String||
|generation|String||
|emailAddresses|[typedEmailAddress](../resources/typedemailaddress.md) collection||
|websites|[website](../resources/website.md) collection||
|imAddresses|String collection||
|jobTitle|String||
|companyName|String||
|department|String||
|officeLocation|String||
|profession|String||
|assistantName|String||
|manager|String||
|phones|[phone](../resources/phone.md) collection||
|postalAddresses|[physicalAddress](../resources/physicaladdress.md) collection||
|spouseName|String||
|personalNotes|String||
|children|String collection||
|weddingAnniversary|Date||
|gender|String||
|isFavorite|Boolean||
|flag|[followupFlag](../resources/followupflag.md)||



## Response
If successful, this method returns a `201 Created` response code and a [contact](../resources/contact.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_contact_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/contacts
Content-type: application/json
Content-length: 2493

{
  "@odata.type": "#microsoft.graph.contact",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "parentFolderId": "Parent Folder Id value",
  "birthday": "2017-01-01T00:00:04.2178204+00:00",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2665

{
  "@odata.type": "#microsoft.graph.contact",
  "id": "9fac6af2-6af2-9fac-f26a-ac9ff26aac9f",
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "parentFolderId": "Parent Folder Id value",
  "birthday": "2017-01-01T00:00:04.2178204+00:00",
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
```

