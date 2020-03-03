---
title: "Add educationalActivities"
description: "Add educationalActivities by posting to the educationalActivities collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add educationalActivities

Namespace: microsoft.graph

Add educationalActivities by posting to the educationalActivities collection.

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
POST /me/profile/educationalActivities/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [educationalActivity](../resources/educationalactivity.md) object.

The following table shows the properties that are required when you create the [educationalActivity](../resources/educationalactivity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|completionMonthYear|Date||
|endMonthYear|Date||
|institution|[institutionData](../resources/institutiondata.md)||
|program|[educationalActivityDetail](../resources/educationalactivitydetail.md)||
|startMonthYear|Date||



## Response
If successful, this method returns a `201 Created` response code and a [educationalActivity](../resources/educationalactivity.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationalactivity_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/profile/educationalActivities
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalactivity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1766

{
  "@odata.type": "#microsoft.graph.educationalActivity",
  "id": "e4f9f389-f389-e4f9-89f3-f9e489f3f9e4",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
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
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
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

