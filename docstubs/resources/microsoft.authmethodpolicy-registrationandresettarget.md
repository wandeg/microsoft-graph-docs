---
title: "registrationAndResetTarget resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# registrationAndResetTarget resource type


Namespace: microsoft.authMethodPolicy



## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String||
|minAuthMethodsToRegister|Int32||
|minAuthMethodsToReset|Int32||
|targetType|Enumeration| Possible values are: `user`, `group`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.authMethodPolicy.registrationAndResetTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.registrationAndResetTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "minAuthMethodsToRegister": 1024,
  "minAuthMethodsToReset": 1024
}
```

