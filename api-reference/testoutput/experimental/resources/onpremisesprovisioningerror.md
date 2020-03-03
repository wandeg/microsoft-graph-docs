---
title: "onPremisesProvisioningError resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# onPremisesProvisioningError resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|String||
|occurredDateTime|DateTimeOffset||
|propertyCausingError|String||
|value|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesProvisioningError",
  "value": "String",
  "category": "String",
  "propertyCausingError": "String",
  "occurredDateTime": "String (timestamp)"
}
```

