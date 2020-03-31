---
title: "Add names"
description: "Add names by posting to the names collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add names

Namespace: microsoft.graph

Add names by posting to the names collection.

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
POST /me/profile/names/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [personName](../resources/personname.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_personname_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/names
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
  "truncated": true,
  "@odata.type": "microsoft.graph.personname"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1245

{
  "@odata.type": "#microsoft.graph.personName",
  "id": "eda5dff1-dff1-eda5-f1df-a5edf1dfa5ed",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
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
  "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00",
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

