---
title: "Add languages"
description: "Add languages by posting to the languages collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add languages

Namespace: microsoft.graph

Add languages by posting to the languages collection.

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
POST /me/profile/languages/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [languageProficiency](../resources/languageproficiency.md) object.

The following table shows the properties that are required when you create the [languageProficiency](../resources/languageproficiency.md).

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
|tag|String||
|proficiency|Enumeration| Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [languageProficiency](../resources/languageproficiency.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_languageproficiency_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/languages
Content-type: application/json
Content-length: 701

{
  "@odata.type": "#microsoft.graph.languageProficiency",
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
  "tag": "Tag value",
  "proficiency": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageproficiency"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 952

{
  "@odata.type": "#microsoft.graph.languageProficiency",
  "id": "1d828f45-8f45-1d82-458f-821d458f821d",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
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
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "displayName": "Display Name value",
  "tag": "Tag value",
  "proficiency": "String"
}
```

