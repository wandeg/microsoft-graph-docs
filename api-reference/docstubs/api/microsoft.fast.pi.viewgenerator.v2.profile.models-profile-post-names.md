---
title: "Create names"
description: "Create a new names object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create names

Namespace: Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models

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
POST /user/{userId}/profile/names
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [personName](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-personname.md) object.

The following table shows the properties that are required when you create the [personName](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-personname.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
|allowedAudiences|allowedAudiences|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-inferencedata.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
|createdBy|[identitySet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
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
|pronunciation|[yomiPersonName](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-yomipersonname.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [personName](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-personname.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_personname_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/user/{userId}/profile/names
Content-Type: application/json
Content-length: 1232

{
  "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.personName",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdBy": {
    "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identitySet",
    "application": {
      "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identity"
    },
    "user": {
      "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identity"
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
    "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.yomiPersonName"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.fast.pi.viewgenerator.v2.profile.models.personname"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.personName",
  "id": "4491a1b5-a1b5-4491-b5a1-9144b5a19144",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2016-12-31T23:59:45.9448095+03:00",
  "createdBy": {
    "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identitySet",
    "application": {
      "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identity"
    },
    "user": {
      "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identity"
    }
  },
  "lastModifiedDateTime": "2017-01-01T00:00:42.7561162+03:00",
  "lastModifiedBy": {
    "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identitySet"
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
    "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.yomiPersonName"
  }
}
```

