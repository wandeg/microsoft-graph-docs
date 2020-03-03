---
title: "informationProtectionContentLabel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# informationProtectionContentLabel resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentMethod|Enumeration|. Possible values are: `standard`, `privileged`, `auto`.|
|creationDateTime|DateTimeOffset||
|label|[labelDetails](../resources/labelDetails.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.informationProtectionContentLabel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.informationProtectionContentLabel",
  "creationDateTime": "String (timestamp)",
  "assignmentMethod": "String",
  "label": {
    "@odata.type": "microsoft.graph.labelDetails",
    "id": "String",
    "name": "String",
    "description": "String",
    "color": "String",
    "sensitivity": 1024,
    "tooltip": "String",
    "isActive": true
  }
}
```

