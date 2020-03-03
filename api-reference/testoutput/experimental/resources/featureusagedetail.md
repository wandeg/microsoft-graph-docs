---
title: "featureUsageDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# featureUsageDetail resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|featureName|String||
|lastConfiguredDateTime|DateTimeOffset||
|lastUsedDateTime|DateTimeOffset||
|licenseAssigned|Enumeration|. Possible values are: `none`, `free`, `basic`, `premiumP1`, `premiumP2`, `unknownFutureValue`.|
|licenseRequired|Enumeration|. Possible values are: `none`, `free`, `basic`, `premiumP1`, `premiumP2`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.featureUsageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.featureUsageDetail",
  "featureName": "String",
  "licenseRequired": "String",
  "licenseAssigned": "String",
  "lastUsedDateTime": "String (timestamp)",
  "lastConfiguredDateTime": "String (timestamp)"
}
```

