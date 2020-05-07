---
title: "deviceHealthScriptRemediationSummary resource type"
description: "The number of device health scripts deployed and the number of devices the scripts remediated."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScriptRemediationSummary resource type


Namespace: microsoft.graph

The number of device health scripts deployed and the number of devices the scripts remediated.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|remediatedDeviceCount|Int32|The number of devices remediated by device health scripts.|
|scriptCount|Int32|The number of device health scripts deployed.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.deviceHealthScriptRemediationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.deviceHealthScriptRemediationSummary",
  "scriptCount": "Integer",
  "remediatedDeviceCount": "Integer"
}
```

