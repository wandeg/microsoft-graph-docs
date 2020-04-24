---
title: "deliveryOptimizationGroupIdSourceOptions resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deliveryOptimizationGroupIdSourceOptions resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [deliveryOptimizationGroupIdSource](../resources/deliveryoptimizationgroupidsource.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|groupIdSourceOption|deliveryOptimizationGroupIdOptionsType|Set this policy to restrict peer selection to a specific source. Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.|

## Relationships
None

## JSON representation
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

