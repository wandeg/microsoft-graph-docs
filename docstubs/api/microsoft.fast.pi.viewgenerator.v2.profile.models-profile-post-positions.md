---
title: "Create positions"
description: "Create a new positions object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create positions

Namespace: Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models

Create a new positions object.

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
POST /user/{userId}/profile/positions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [workPosition](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-workposition.md) object.

The following table shows the properties that are required when you create the [workPosition](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-workposition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
|allowedAudiences|allowedAudiences|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-inferencedata.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
|createdBy|[identitySet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-itemfacet.md)|
|categories|String collection|**TODO: Add Description**|
|detail|[positionDetail](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-positiondetail.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [workPosition](../resources/microsoft.fast.pi.viewgenerator.v2.profile.models-workposition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workposition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/user/{userId}/profile/positions
Content-Type: application/json
Content-length: 1859

{
  "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.workPosition",
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
  "categories": [
    "Categories value"
  ],
  "detail": {
    "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.positionDetail",
    "company": {
      "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.companyDetail",
      "pronunciation": "Pronunciation value",
      "department": "Department value",
      "officeLocation": "Office Location value",
      "address": {
        "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.physicalAddress",
        "type": "String",
        "postOfficeBox": "Post Office Box value",
        "street": "Street value",
        "city": "City value",
        "state": "State value",
        "countryOrRegion": "Country Or Region value",
        "postalCode": "Postal Code value"
      },
      "webUrl": "https://example.com/webUrl/"
    },
    "description": "Description value",
    "endMonthYear": "Date",
    "jobTitle": "Job Title value",
    "role": "Role value",
    "startMonthYear": "Date",
    "summary": "Summary value"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.fast.pi.viewgenerator.v2.profile.models.workposition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.workPosition",
  "id": "175e17de-17de-175e-de17-5e17de175e17",
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
  "categories": [
    "Categories value"
  ],
  "detail": {
    "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.positionDetail",
    "company": {
      "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.companyDetail",
      "pronunciation": "Pronunciation value",
      "department": "Department value",
      "officeLocation": "Office Location value",
      "address": {
        "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.physicalAddress",
        "type": "String",
        "postOfficeBox": "Post Office Box value",
        "street": "Street value",
        "city": "City value",
        "state": "State value",
        "countryOrRegion": "Country Or Region value",
        "postalCode": "Postal Code value"
      },
      "webUrl": "https://example.com/webUrl/"
    },
    "description": "Description value",
    "endMonthYear": "Date",
    "jobTitle": "Job Title value",
    "role": "Role value",
    "startMonthYear": "Date",
    "summary": "Summary value"
  }
}
```

