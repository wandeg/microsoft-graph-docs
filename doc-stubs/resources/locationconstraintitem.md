---
title: "locationConstraintItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# locationConstraintItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [location](../resources/location.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description** Inherited from [location](../resources/location.md)|
|coordinates|[outlookGeoCoordinates](../resources/outlookgeocoordinates.md)|**TODO: Add Description** Inherited from [location](../resources/location.md)|
|displayName|String|**TODO: Add Description** Inherited from [location](../resources/location.md)|
|locationEmailAddress|String|**TODO: Add Description** Inherited from [location](../resources/location.md)|
|locationType|locationType|**TODO: Add Description** Inherited from [location](../resources/location.md). Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`, `geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.|
|locationUri|String|**TODO: Add Description** Inherited from [location](../resources/location.md)|
|resolveAvailability|Boolean|**TODO: Add Description**|
|uniqueId|String|**TODO: Add Description** Inherited from [location](../resources/location.md)|
|uniqueIdType|locationUniqueIdType|**TODO: Add Description** Inherited from [location](../resources/location.md). Possible values are: `unknown`, `locationStore`, `directory`, `private`, `bing`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationConstraintItem",
  "displayName": "String",
  "locationEmailAddress": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "coordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates"
  },
  "locationUri": "String",
  "locationType": "String",
  "uniqueId": "String",
  "uniqueIdType": "String",
  "resolveAvailability": "Boolean"
}
```

