---
title: "Create projects"
description: "Create a new projects object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create projects

Namespace: microsoft.graph

Create a new projects object.

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
POST /invitations/{invitationsId}/invitedUser/profile/projects
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [projectParticipation](../resources/projectparticipation.md) object.

The following table shows the properties that are required when you create the [projectParticipation](../resources/projectparticipation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|allowedAudiences|allowedAudiences|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/inferencedata.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|categories|String collection|**TODO: Add Description**|
|client|[companyDetail](../resources/companydetail.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|detail|[positionDetail](../resources/positiondetail.md)|**TODO: Add Description**|
|colleagues|[relatedPerson](../resources/relatedperson.md) collection|**TODO: Add Description**|
|sponsors|[relatedPerson](../resources/relatedperson.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [projectParticipation](../resources/projectparticipation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_projectparticipation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/profile/projects
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectparticipation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.projectParticipation",
  "id": "76504ca6-4ca6-7650-a64c-5076a64c5076",
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

