---
title: "licenseInfoDetail resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# licenseInfoDetail resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|licenseType|azureADLicenseType|**TODO: Add Description**. Possible values are: `none`, `free`, `basic`, `premiumP1`, `premiumP2`, `unknownFutureValue`.|
|totalAssignedCount|Int32|**TODO: Add Description**|
|totalLicenseCount|Int32|**TODO: Add Description**|
|totalUsageCount|Int32|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.licenseInfoDetail"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.licenseInfoDetail",
  "licenseType": "String",
  "totalLicenseCount": 1024,
  "totalAssignedCount": 1024,
  "totalUsageCount": 1024
}
```

