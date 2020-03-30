---
title: "Update languageProficiency"
description: "Update the properties of a languageProficiency object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update languageProficiency

Namespace: microsoft.graph

Update the properties of a [languageProficiency](../resources/languageproficiency.md) object.

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
PATCH /me/profile/languages/{languageProficiencyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_languageproficiency"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile/languages/{languageProficiencyId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 952

{
  "@odata.type": "#microsoft.graph.languageProficiency",
  "id": "acc19991-9991-acc1-9199-c1ac9199c1ac",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
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
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "displayName": "Display Name value",
  "tag": "Tag value",
  "proficiency": "String"
}
```

