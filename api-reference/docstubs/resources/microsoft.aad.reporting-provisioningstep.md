---
title: "provisioningStep resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# provisioningStep resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|details|[detailsInfo](../resources/microsoft.aad.reporting-detailsinfo.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|provisioningStepType|provisioningStepType|**TODO: Add Description**. Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.|
|status|provisioningResult|**TODO: Add Description**. Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.|

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

