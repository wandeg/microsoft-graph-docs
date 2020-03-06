---
title: "userRegistrationCount resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userRegistrationCount resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|registrationCount|Int64||
|registrationStatus|Enumeration|. Possible values are: `registered`, `enabled`, `capable`, `mfaRegistered`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationCount",
  "registrationStatus": "String",
  "registrationCount": 1024
}
```

