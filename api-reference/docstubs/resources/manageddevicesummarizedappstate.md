---
title: "managedDeviceSummarizedAppState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedDeviceSummarizedAppState resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceId|String|DeviceId of device represented by this object|
|summarizedAppState|runState|runState for the object. Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceSummarizedAppState",
  "summarizedAppState": "String",
  "deviceId": "String"
}
```

