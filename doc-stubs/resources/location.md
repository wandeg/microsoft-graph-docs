---
title: "location resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# location resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|coordinates|[outlookGeoCoordinates](../resources/outlookgeocoordinates.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|locationEmailAddress|String|**TODO: Add Description**|
|locationType|locationType|**TODO: Add Description**. Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`, `geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.|
|locationUri|String|**TODO: Add Description**|
|uniqueId|String|**TODO: Add Description**|
|uniqueIdType|locationUniqueIdType|**TODO: Add Description**. Possible values are: `unknown`, `locationStore`, `directory`, `private`, `bing`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.location"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.location",
  "displayName": "String",
  "locationEmailAddress": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "locationUri": "String",
  "coordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates"
  },
  "locationType": "String",
  "uniqueId": "String",
  "uniqueIdType": "String"
}
```

