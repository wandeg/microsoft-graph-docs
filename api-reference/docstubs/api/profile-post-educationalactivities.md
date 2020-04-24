---
title: "Create educationalActivities"
description: "Create a new educationalActivities object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create educationalActivities

Namespace: microsoft.graph

Create a new educationalActivities object.

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
POST /invitations/{invitationsId}/invitedUser/profile/educationalActivities
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [educationalActivity](../resources/educationalactivity.md) object.

The following table shows the properties that are required when you create the [educationalActivity](../resources/educationalactivity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|allowedAudiences|allowedAudiences|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/inferencedata.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
|completionMonthYear|Date|**TODO: Add Description**|
|endMonthYear|Date|**TODO: Add Description**|
|institution|[institutionData](../resources/institutiondata.md)|**TODO: Add Description**|
|program|[educationalActivityDetail](../resources/educationalactivitydetail.md)|**TODO: Add Description**|
|startMonthYear|Date|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [educationalActivity](../resources/educationalactivity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationalactivity_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/profile/educationalActivities
Content-Type: application/json
Content-length: 1516

{
  "@odata.type": "#microsoft.graph.educationalActivity",
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
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "@odata.type": "microsoft.graph.institutionData",
    "description": "Description value",
    "location": {
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
  "program": {
    "@odata.type": "microsoft.graph.educationalActivityDetail",
    "abbreviation": "Abbreviation value",
    "activities": "Activities value",
    "awards": "Awards value",
    "fieldsOfStudy": "Fields Of Study value",
    "grade": "Grade value",
    "notes": "Notes value"
  },
  "startMonthYear": "Date"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalactivity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.educationalActivity",
  "id": "095c77cc-77cc-095c-cc77-5c09cc775c09",
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
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "@odata.type": "microsoft.graph.institutionData",
    "description": "Description value",
    "location": {
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
  "program": {
    "@odata.type": "microsoft.graph.educationalActivityDetail",
    "abbreviation": "Abbreviation value",
    "activities": "Activities value",
    "awards": "Awards value",
    "fieldsOfStudy": "Fields Of Study value",
    "grade": "Grade value",
    "notes": "Notes value"
  },
  "startMonthYear": "Date"
}
```

