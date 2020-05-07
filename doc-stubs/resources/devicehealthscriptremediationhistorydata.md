---
title: "deviceHealthScriptRemediationHistoryData resource type"
description: "The number of devices remediated by a device health script on a given date."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScriptRemediationHistoryData resource type


Namespace: microsoft.graph

The number of devices remediated by a device health script on a given date.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|date|Date|The date on which devices were remediated by the device health script.|
|noIssueDeviceCount|Int32|The number of devices that were found to have no issue by the device health script.|
|remediatedDeviceCount|Int32|The number of devices remediated by the device health script.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.deviceHealthScriptRemediationHistoryData"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.deviceHealthScriptRemediationHistoryData",
  "date": "Date",
  "remediatedDeviceCount": "Integer",
  "noIssueDeviceCount": "Integer"
}
```

