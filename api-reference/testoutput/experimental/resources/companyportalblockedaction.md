---
title: "companyPortalBlockedAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# companyPortalBlockedAction resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|Enumeration|Device Action. Possible values are: `unknown`, `remove`, `reset`.|
|ownerType|Enumeration|Device ownership type. Possible values are: `unknown`, `company`, `personal`.|
|platform|Enumeration|Device OS/Platform. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.companyPortalBlockedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyPortalBlockedAction",
  "platform": "String",
  "ownerType": "String",
  "action": "String"
}
```

