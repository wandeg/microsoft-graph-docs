---
title: "educationSynchronizationCustomization resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationSynchronizationCustomization resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowDisplayNameUpdate|Boolean||
|isSyncDeferred|Boolean||
|optionalPropertiesToSync|String collection||
|synchronizationStartDate|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomization",
  "optionalPropertiesToSync": [
    "String"
  ],
  "synchronizationStartDate": "String (timestamp)",
  "isSyncDeferred": true,
  "allowDisplayNameUpdate": true
}
```

