---
title: "licenseInfoDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# licenseInfoDetail resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|licenseType|Enumeration| Possible values are: `none`, `free`, `basic`, `premiumP1`, `premiumP2`, `unknownFutureValue`.|
|totalAssignedCount|Int32||
|totalLicenseCount|Int32||
|totalUsageCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.licenseInfoDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.licenseInfoDetail",
  "licenseType": "String",
  "totalLicenseCount": 1024,
  "totalAssignedCount": 1024,
  "totalUsageCount": 1024
}
```

