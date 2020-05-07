---
title: "osVersionCount resource type"
description: "Count of devices with malware for each OS version"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# osVersionCount resource type


Namespace: microsoft.graph

Count of devices with malware for each OS version

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceCount|Int32|Count of devices with malware for the OS version|
|lastUpdateDateTime|DateTimeOffset|The Timestamp of the last update for the device count in UTC|
|osVersion|String|OS version|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.osVersionCount",
  "osVersion": "String",
  "deviceCount": "Integer",
  "lastUpdateDateTime": "String (timestamp)"
}
```

