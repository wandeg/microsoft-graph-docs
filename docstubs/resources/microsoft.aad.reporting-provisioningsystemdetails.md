---
title: "provisioningSystemDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# provisioningSystemDetails resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|details|[detailsInfo](../resources/microsoft.aad.reporting-detailsinfo.md)||
|displayName|String||
|id|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.provisioningSystemDetails",
  "id": "String (identifier)",
  "displayName": "String",
  "details": {
    "@odata.type": "Microsoft.AAD.Reporting.detailsInfo"
  }
}
```

