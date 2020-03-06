---
title: "educationalActivity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationalActivity resource type


Namespace: microsoft.graph




Inherits from [itemFacet](../resources/itemfacet.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationalActivity](../api/educationalactivity-get.md)|[educationalActivity](../resources/educationalactivity.md)|Read properties and relationships of the [educationalActivity](../resources/educationalactivity.md) object.|
|[Update educationalActivity](../api/educationalactivity-update.md)|[educationalActivity](../resources/educationalactivity.md)|Update the properties of a [educationalActivity](../resources/educationalactivity.md) object.|
|[List educationalActivities](../api/profile-list-educationalactivities.md)|[educationalActivity](../resources/educationalactivity.md) collection|Get the educationalActivities from the educationalActivities navigation property.|
|[Add educationalActivities](../api/profile-post-educationalactivities.md)|[educationalActivity](../resources/educationalactivity.md)|Add educationalActivities by posting to the educationalActivities collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|completionMonthYear|Date||
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|endMonthYear|Date||
|id|String| Inherited from [entity](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|institution|[institutionData](../resources/institutiondata.md)||
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|program|[educationalActivityDetail](../resources/educationalactivitydetail.md)||
|startMonthYear|Date||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationalActivity",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationalActivity",
  "id": "String (identifier)",
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

