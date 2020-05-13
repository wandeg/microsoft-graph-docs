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
POST /user/{userId}/profile/educationalActivities
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [educationalActivity](../resources/educationalactivity.md) object.

The following table shows the properties that are required when you create the [educationalActivity](../resources/educationalactivity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md)|
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
POST https://graph.microsoft.com/beta/user/{userId}/profile/educationalActivities
Content-Type: application/json
Content-length: 534

{
  "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.educationalActivity",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "@odata.type": "microsoft.graph.institutionData"
  },
  "program": {
    "@odata.type": "microsoft.graph.educationalActivityDetail"
  },
  "startMonthYear": "Date"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.fast.pi.viewgenerator.v2.profile.models.educationalactivity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.educationalActivity",
  "id": "9660a0cb-a0cb-9660-cba0-6096cba06096",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "@odata.type": "microsoft.graph.institutionData"
  },
  "program": {
    "@odata.type": "microsoft.graph.educationalActivityDetail"
  },
  "startMonthYear": "Date"
}
```

