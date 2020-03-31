---
title: "appFamilyDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appFamilyDetails resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|groupDisplayName|String||
|groupId|String||
|status|Enumeration| Possible values are: `OptOut`, `OptIn`, `NotProvisioned`, `OptIn_Selected`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appFamilyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appFamilyDetails",
  "status": "String",
  "groupDisplayName": "String",
  "groupId": "String"
}
```

