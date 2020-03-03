---
title: "mobileAppInstallTimeSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# mobileAppInstallTimeSettings resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|deadlineDateTime|DateTimeOffset|The time at which the app should be installed.|
|startDateTime|DateTimeOffset|The time at which the app should be available for installation.|
|useLocalTime|Boolean|Whether the local device time or UTC time should be used when determining the available and deadline times.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallTimeSettings",
  "useLocalTime": true,
  "startDateTime": "String (timestamp)",
  "deadlineDateTime": "String (timestamp)"
}
```

