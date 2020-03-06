---
title: "provisioningStep resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# provisioningStep resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|details|[detailsInfo](../resources/detailsinfo.md)||
|name|String||
|provisioningStepType|Enumeration|. Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.|
|status|Enumeration|. Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.provisioningStep"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.provisioningStep",
  "name": "String",
  "status": "String",
  "description": "String",
  "details": {
    "@odata.type": "microsoft.graph.detailsInfo"
  },
  "provisioningStepType": "String"
}
```

