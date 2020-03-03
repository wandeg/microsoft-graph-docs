---
title: "assignedPlan resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# assignedPlan resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedDateTime|DateTimeOffset||
|capabilityStatus|String||
|service|String||
|servicePlanId|Guid||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignedPlan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignedPlan",
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "String",
  "service": "String",
  "servicePlanId": "Guid"
}
```

