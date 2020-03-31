---
title: "Update personName"
description: "Update the properties of a personName object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update personName

Namespace: microsoft.graph

Update the properties of a [personName](../resources/personname.md) object.

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
PATCH /me/profile/names/{personNameId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [personName](../resources/personname.md) object.

The following table shows the properties that are required when you create the [personName](../resources/personname.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|displayName|String||
|first|String||
|initials|String||
|last|String||
|languageTag|String||
|maiden|String||
|middle|String||
|nickname|String||
|suffix|String||
|title|String||
|pronunciation|[yomiPersonName](../resources/yomipersonname.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_personname"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile/names/{personNameId}
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1244

{
  "@odata.type": "#microsoft.graph.personName",
  "id": "12c7e3e6-e3e6-12c7-e6e3-c712e6e3c712",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
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
  "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00",
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

