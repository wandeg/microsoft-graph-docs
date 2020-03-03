---
title: "vppTokenLicenseSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# vppTokenLicenseSummary resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleId|String|The Apple Id associated with the given Apple Volume Purchase Program Token.|
|availableLicenseCount|Int32|The number of VPP licenses available.|
|organizationName|String|The organization associated with the Apple Volume Purchase Program Token.|
|usedLicenseCount|Int32|The number of VPP licenses in use.|
|vppTokenId|String|Identifier of the VPP token.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```

