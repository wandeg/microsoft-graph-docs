---
title: "provisionedIdentity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# provisionedIdentity resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|details|[detailsInfo](../resources/microsoft.aad.reporting-detailsinfo.md)||
|displayName|String||
|id|String||
|identityType|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.provisionedIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "identityType": "String",
  "details": {
    "@odata.type": "Microsoft.AAD.Reporting.detailsInfo"
  }
}
```

