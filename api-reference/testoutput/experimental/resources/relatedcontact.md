---
title: "relatedContact resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# relatedContact resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessConsent|Boolean||
|displayName|String||
|emailAddress|String||
|id|String||
|mobilePhone|String||
|relationship|Enumeration|. Possible values are: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.relatedContact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.relatedContact",
  "id": "String (identifier)",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "String",
  "accessConsent": true
}
```

