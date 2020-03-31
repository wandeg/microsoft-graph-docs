---
title: "Add projects"
description: "Add projects by posting to the projects collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add projects

Namespace: microsoft.graph

Add projects by posting to the projects collection.

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
POST /me/profile/projects/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [projectParticipation](../resources/projectparticipation.md) object.

The following table shows the properties that are required when you create the [projectParticipation](../resources/projectparticipation.md).

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
|client|[companyDetail](../resources/companydetail.md)||
|displayName|String||
|detail|[positionDetail](../resources/positiondetail.md)||
|colleagues|[relatedPerson](../resources/relatedperson.md) collection||
|sponsors|[relatedPerson](../resources/relatedperson.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [projectParticipation](../resources/projectparticipation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_projectparticipation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/projects
Content-type: application/json
Content-length: 1920

{
  "@odata.type": "#microsoft.graph.projectParticipation",
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
  "client": {
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
  "displayName": "Display Name value",
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail",
    "company": {
      "@odata.type": "microsoft.graph.companyDetail"
    },
    "description": "Description value",
    "endMonthYear": "Date",
    "jobTitle": "Job Title value",
    "role": "Role value",
    "startMonthYear": "Date",
    "summary": "Summary value"
  },
  "colleagues": [
    {
      "@odata.type": "microsoft.graph.relatedPerson",
      "relationship": "String",
      "userPrincipalName": "User Principal Name value"
    }
  ],
  "sponsors": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectparticipation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2170

{
  "@odata.type": "#microsoft.graph.projectParticipation",
  "id": "82eb990a-990a-82eb-0a99-eb820a99eb82",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
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
  "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "categories": [
    "Categories value"
  ],
  "client": {
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
  "displayName": "Display Name value",
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail",
    "company": {
      "@odata.type": "microsoft.graph.companyDetail"
    },
    "description": "Description value",
    "endMonthYear": "Date",
    "jobTitle": "Job Title value",
    "role": "Role value",
    "startMonthYear": "Date",
    "summary": "Summary value"
  },
  "colleagues": [
    {
      "@odata.type": "microsoft.graph.relatedPerson",
      "relationship": "String",
      "userPrincipalName": "User Principal Name value"
    }
  ],
  "sponsors": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ]
}
```

