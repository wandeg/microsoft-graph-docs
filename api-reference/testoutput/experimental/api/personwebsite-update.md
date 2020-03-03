---
title: "Update personWebsite"
description: "Update the properties of a personWebsite object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update personWebsite

Update the properties of a [personWebsite](../resources/personwebsite.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/websites/{personWebsiteId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [personWebsite](../resources/personWebsite.md) object.

The following table shows the properties that are required when you create the [personWebsite](../resources/personwebsite.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemFacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/inferenceData.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemFacet.md)|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemFacet.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|categories|String collection||
|description|String||
|displayName|String||
|webUrl|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [personWebsite](../resources/personwebsite.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_personwebsite"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/me/profile/websites/{personWebsiteId}
Content-type: application/json
Content-length: 776

{
  "@odata.type": "#microsoft.graph.personWebsite",
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
  "categories": [
    "Categories value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "webUrl": "https://example.com/webUrl/"
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
Content-Length: 1027

{
  "@odata.type": "#microsoft.graph.personWebsite",
  "id": "872dcede-cede-872d-dece-2d87dece2d87",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
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
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "categories": [
    "Categories value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "webUrl": "https://example.com/webUrl/"
}
```

