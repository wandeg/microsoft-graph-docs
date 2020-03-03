---
title: "managedDeviceOverview resource type"
description: "Summary data for managed devices"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedDeviceOverview resource type


Namespace: microsoft.graph

Summary data for managed devices


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedDeviceOverviews](../api/intune-devices-manageddeviceoverview-list.md)|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) collection|List properties and relationships of the [managedDeviceOverview](../resources/manageddeviceoverview.md) objects.|
|[Get managedDeviceOverview](../api/intune-devices-manageddeviceoverview-get.md)|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.|
|[Create managedDeviceOverview](../api/intune-devices-manageddeviceoverview-create.md)|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Create a new [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.|
|[Delete managedDeviceOverview](../api/intune-devices-manageddeviceoverview-delete.md)|None|Deletes a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).|
|[Update managedDeviceOverview](../api/intune-devices-manageddeviceoverview-update.md)|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceExchangeAccessStateSummary|[deviceExchangeAccessStateSummary](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|Distribution of Exchange Access State in Intune|
|deviceOperatingSystemSummary|[deviceOperatingSystemSummary](../resources/intune-devices-deviceoperatingsystemsummary.md)|Device operating system summary.|
|dualEnrolledDeviceCount|Int32|The number of devices enrolled in both MDM and EAS|
|enrolledDeviceCount|Int32|Total enrolled device count. Does not include PC devices managed via Intune PC Agent|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified date time of device overview|
|managedDeviceModelsAndManufacturers|[managedDeviceModelsAndManufacturers](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|Models and Manufactures meatadata for managed devices in the account|
|mdmEnrolledCount|Int32|The number of devices enrolled in MDM|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

