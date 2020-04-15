---
title: "provisioningStep resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# provisioningStep resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|details|[detailsInfo](../resources/microsoft.aad.reporting-detailsinfo.md)||
|name|String||
|provisioningStepType|Enumeration| Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.|
|status|Enumeration| Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.provisioningStep"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.provisioningStep",
  "name": "String",
  "status": "String",
  "description": "String",
  "details": {
    "@odata.type": "Microsoft.AAD.Reporting.detailsInfo"
  },
  "provisioningStepType": "String"
}
```

