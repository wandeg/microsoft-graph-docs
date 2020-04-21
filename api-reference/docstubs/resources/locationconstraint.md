---
title: "locationConstraint resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# locationConstraint resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|isRequired|Boolean|**TODO: Add Description**|
|locations|[locationConstraintItem](../resources/locationconstraintitem.md) collection|**TODO: Add Description**|
|suggestLocation|Boolean|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locationConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationConstraint",
  "locations": [
    {
      "@odata.type": "microsoft.graph.locationConstraintItem",
      "displayName": "String",
      "locationEmailAddress": "String",
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress",
        "street": "String",
        "city": "String",
        "state": "String",
        "countryOrRegion": "String",
        "postalCode": "String"
      },
      "locationUri": "String",
      "coordinates": {
        "@odata.type": "microsoft.graph.outlookGeoCoordinates",
        "latitude": "Double",
        "longitude": "Double",
        "accuracy": "Double",
        "altitude": "Double",
        "altitudeAccuracy": "Double"
      },
      "locationType": "String",
      "uniqueId": "String",
      "uniqueIdType": "String",
      "resolveAvailability": true
    }
  ],
  "isRequired": true,
  "suggestLocation": true
}
```

