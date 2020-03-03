---
title: "cloudAppSecuritySessionControl resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# cloudAppSecuritySessionControl resource type


Namespace: microsoft.graph




Inherits from [conditionalAccessSessionControl](../resources/conditionalaccesssessioncontrol.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|cloudAppSecurityType|Enumeration|. Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.|
|isEnabled|Boolean| Inherited from [conditionalAccessSessionControl](../resources/conditionalaccesssessioncontrol.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudAppSecuritySessionControl"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudAppSecuritySessionControl",
  "isEnabled": true,
  "cloudAppSecurityType": "String"
}
```

