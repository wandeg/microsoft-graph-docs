---
title: "Update workPosition"
description: "Update the properties of a workPosition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workPosition

Namespace: microsoft.graph

Update the properties of a [workPosition](../resources/workposition.md) object.

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
PATCH /me/profile/positions/{workPositionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workPosition](../resources/workposition.md) object.

The following table shows the properties that are required when you create the [workPosition](../resources/workposition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|categories|String collection||
|detail|[positionDetail](../resources/positiondetail.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [workPosition](../resources/workposition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workposition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile/positions/{workPositionId}
Content-type: application/json
Content-length: 1553

{
  "@odata.type": "#microsoft.graph.workPosition",
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
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail",
    "company": {
      "@odata.type": "microsoft.graph.companyDetail",
      "pronunciation": "Pronunciation value",
      "department": "Department value",
      "officeLocation": "Office Location value",
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1804

{
  "@odata.type": "#microsoft.graph.workPosition",
  "id": "2850c339-c339-2850-39c3-502839c35028",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
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
  "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "categories": [
    "Categories value"
  ],
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail",
    "company": {
      "@odata.type": "microsoft.graph.companyDetail",
      "pronunciation": "Pronunciation value",
      "department": "Department value",
      "officeLocation": "Office Location value",
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress",
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

