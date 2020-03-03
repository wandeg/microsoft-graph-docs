---
title: "managedAppDiagnosticStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedAppDiagnosticStatus resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|mitigationInstruction|String|Instruction on how to mitigate a failed validation|
|state|String|The state of the operation|
|validationName|String|The validation friendly name|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```

