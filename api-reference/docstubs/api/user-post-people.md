---
title: "Create people"
description: "Create a new people object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create people

Namespace: microsoft.graph

Create a new people object.

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
POST /me/people
POST /users/{usersId}/people
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [person](../resources/person.md) object.

The following table shows the properties that are required when you create the [person](../resources/person.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|birthday|String|**TODO: Add Description**|
|personNotes|String|**TODO: Add Description**|
|isFavorite|Boolean|**TODO: Add Description**|
|emailAddresses|[rankedEmailAddress](../resources/rankedemailaddress.md) collection|**TODO: Add Description**|
|phones|[phone](../resources/phone.md) collection|**TODO: Add Description**|
|postalAddresses|[location](../resources/location.md) collection|**TODO: Add Description**|
|websites|[website](../resources/website.md) collection|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|yomiCompany|String|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|profession|String|**TODO: Add Description**|
|sources|[personDataSource](../resources/persondatasource.md) collection|**TODO: Add Description**|
|mailboxType|String|**TODO: Add Description**|
|personType|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [person](../resources/person.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_person_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/people
Content-Type: application/json
Content-length: 913

{
  "@odata.type": "#microsoft.graph.person",
  "displayName": "String",
  "givenName": "String",
  "surname": "String",
  "birthday": "String",
  "personNotes": "String",
  "isFavorite": "Boolean",
  "emailAddresses": [
    {
      "@odata.type": "microsoft.graph.rankedEmailAddress"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ],
  "postalAddresses": [
    {
      "@odata.type": "microsoft.graph.location"
    }
  ],
  "websites": [
    {
      "@odata.type": "microsoft.graph.website"
    }
  ],
  "title": "String",
  "companyName": "String",
  "yomiCompany": "String",
  "department": "String",
  "officeLocation": "String",
  "profession": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.personDataSource"
    }
  ],
  "mailboxType": "String",
  "personType": "String",
  "userPrincipalName": "String"
}
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
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.person",
  "id": "177ca347-a347-177c-47a3-7c1747a37c17",
  "displayName": "String",
  "givenName": "String",
  "surname": "String",
  "birthday": "String",
  "personNotes": "String",
  "isFavorite": "Boolean",
  "emailAddresses": [
    {
      "@odata.type": "microsoft.graph.rankedEmailAddress"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ],
  "postalAddresses": [
    {
      "@odata.type": "microsoft.graph.location"
    }
  ],
  "websites": [
    {
      "@odata.type": "microsoft.graph.website"
    }
  ],
  "title": "String",
  "companyName": "String",
  "yomiCompany": "String",
  "department": "String",
  "officeLocation": "String",
  "profession": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.personDataSource"
    }
  ],
  "mailboxType": "String",
  "personType": "String",
  "userPrincipalName": "String"
}
```

