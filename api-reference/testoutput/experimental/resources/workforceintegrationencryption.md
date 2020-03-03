---
title: "workforceIntegrationEncryption resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workforceIntegrationEncryption resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|protocol|Enumeration|. Possible values are: `sharedSecret`, `unknownFutureValue`.|
|secret|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.workforceIntegrationEncryption"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workforceIntegrationEncryption",
  "protocol": "String",
  "secret": "String"
}
```

