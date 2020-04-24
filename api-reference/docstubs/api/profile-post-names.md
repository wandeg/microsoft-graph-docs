---
title: "Create names"
description: "Create a new names object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create names

Namespace: microsoft.graph

Create a new names object.

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
POST /invitations/{invitationsId}/invitedUser/profile/names
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [personName](../resources/personname.md) object.

The following table shows the properties that are required when you create the [personName](../resources/personname.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|allowedAudiences|allowedAudiences|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/inferencedata.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|displayName|String|**TODO: Add Description**|
|first|String|**TODO: Add Description**|
|initials|String|**TODO: Add Description**|
|last|String|**TODO: Add Description**|
|languageTag|String|**TODO: Add Description**|
|maiden|String|**TODO: Add Description**|
|middle|String|**TODO: Add Description**|
|nickname|String|**TODO: Add Description**|
|suffix|String|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|pronunciation|[yomiPersonName](../resources/yomipersonname.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [personName](../resources/personname.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_personname_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/profile/names
Content-Type: application/json
Content-length: 994

{
  "@odata.type": "#microsoft.graph.personName",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "displayName": "Display Name value",
  "first": "First value",
  "initials": "Initials value",
  "last": "Last value",
  "languageTag": "Language Tag value",
  "maiden": "Maiden value",
  "middle": "Middle value",
  "nickname": "Nickname value",
  "suffix": "Suffix value",
  "title": "Title value",
  "pronunciation": {
    "@odata.type": "microsoft.graph.yomiPersonName"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personname"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.personName",
  "id": "b07fbd86-bd86-b07f-86bd-7fb086bd7fb0",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "displayName": "Display Name value",
  "first": "First value",
  "initials": "Initials value",
  "last": "Last value",
  "languageTag": "Language Tag value",
  "maiden": "Maiden value",
  "middle": "Middle value",
  "nickname": "Nickname value",
  "suffix": "Suffix value",
  "title": "Title value",
  "pronunciation": {
    "@odata.type": "microsoft.graph.yomiPersonName"
  }
}
```

