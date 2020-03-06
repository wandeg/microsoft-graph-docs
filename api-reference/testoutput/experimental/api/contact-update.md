---
title: "Update contact"
description: "Update the properties of a contact object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update contact

Namespace: microsoft.graph

Update the properties of a [contact](../resources/contact.md) object.

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
PATCH /me/contacts/{contactId}
PATCH /users/{usersId}/contacts/{contactId}
PATCH /me/contactFolders/{contactFolderId}/contacts/{contactId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_contact"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/contacts/{contactId}
Content-type: application/json
Content-length: 2493

{
  "@odata.type": "#microsoft.graph.contact",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "parentFolderId": "Parent Folder Id value",
  "birthday": "2017-01-01T00:00:29.9801848+03:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2665

{
  "@odata.type": "#microsoft.graph.contact",
  "id": "0269e727-e727-0269-27e7-690227e76902",
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "parentFolderId": "Parent Folder Id value",
  "birthday": "2017-01-01T00:00:29.9801848+03:00",
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

