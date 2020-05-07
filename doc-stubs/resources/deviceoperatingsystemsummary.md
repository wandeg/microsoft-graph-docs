---
title: "deviceOperatingSystemSummary resource type"
description: "Device operating system summary."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceOperatingSystemSummary resource type


Namespace: microsoft.graph

Device operating system summary.

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
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.deviceOperatingSystemSummary",
  "androidCount": "Integer",
  "iosCount": "Integer",
  "macOSCount": "Integer",
  "windowsMobileCount": "Integer",
  "windowsCount": "Integer",
  "unknownCount": "Integer",
  "androidDedicatedCount": "Integer",
  "androidDeviceAdminCount": "Integer",
  "androidFullyManagedCount": "Integer",
  "androidWorkProfileCount": "Integer",
  "configMgrDeviceCount": "Integer"
}
```

