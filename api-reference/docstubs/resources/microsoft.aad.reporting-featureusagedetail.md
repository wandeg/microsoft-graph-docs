---
title: "featureUsageDetail resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# featureUsageDetail resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|featureName|String|**TODO: Add Description**|
|lastConfiguredDateTime|DateTimeOffset|**TODO: Add Description**|
|lastUsedDateTime|DateTimeOffset|**TODO: Add Description**|
|licenseAssigned|azureADLicenseType|**TODO: Add Description**. Possible values are: `none`, `free`, `basic`, `premiumP1`, `premiumP2`, `unknownFutureValue`.|
|licenseRequired|azureADLicenseType|**TODO: Add Description**. Possible values are: `none`, `free`, `basic`, `premiumP1`, `premiumP2`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.featureUsageDetail"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.featureUsageDetail",
  "featureName": "String",
  "licenseRequired": "String",
  "licenseAssigned": "String",
  "lastUsedDateTime": "String (timestamp)",
  "lastConfiguredDateTime": "String (timestamp)"
}
```

