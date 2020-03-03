---
title: "deliveryOptimizationGroupIdSourceOptions resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deliveryOptimizationGroupIdSourceOptions resource type


Namespace: microsoft.graph




Inherits from [deliveryOptimizationGroupIdSource](../resources/deliveryoptimizationgroupidsource.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|groupIdSourceOption|Enumeration|Set this policy to restrict peer selection to a specific source. Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSourceOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdSourceOptions",
  "groupIdSourceOption": "String"
}
```

