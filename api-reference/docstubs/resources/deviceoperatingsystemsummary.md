---
title: "deviceOperatingSystemSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceOperatingSystemSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidCount|Int32|Number of android device count.|
|androidDedicatedCount|Int32|Number of dedicated Android devices.|
|androidDeviceAdminCount|Int32|Number of device admin Android devices.|
|androidFullyManagedCount|Int32|Number of fully managed Android devices.|
|androidWorkProfileCount|Int32|Number of work profile Android devices.|
|configMgrDeviceCount|Int32|Number of ConfigMgr managed devices.|
|iosCount|Int32|Number of iOS device count.|
|macOSCount|Int32|Number of Mac OS X device count.|
|unknownCount|Int32|Number of unknown device count.|
|windowsCount|Int32|Number of Windows device count.|
|windowsMobileCount|Int32|Number of Windows mobile device count.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024,
  "androidDedicatedCount": 1024,
  "androidDeviceAdminCount": 1024,
  "androidFullyManagedCount": 1024,
  "androidWorkProfileCount": 1024,
  "configMgrDeviceCount": 1024
}
```

