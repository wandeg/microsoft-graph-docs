---
title: "managedDeviceOverview resource type"
description: "Summary data for managed devices"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedDeviceOverview resource type


Namespace: microsoft.graph

Summary data for managed devices

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceExchangeAccessStateSummary|[deviceExchangeAccessStateSummary](../resources/deviceexchangeaccessstatesummary.md)|Distribution of Exchange Access State in Intune|
|deviceOperatingSystemSummary|[deviceOperatingSystemSummary](../resources/deviceoperatingsystemsummary.md)|Device operating system summary.|
|dualEnrolledDeviceCount|Int32|The number of devices enrolled in both MDM and EAS|
|enrolledDeviceCount|Int32|Total enrolled device count. Does not include PC devices managed via Intune PC Agent|
|id|String|Unique Identifier for the summary|
|lastModifiedDateTime|DateTimeOffset|Last modified date time of device overview|
|managedDeviceModelsAndManufacturers|[managedDeviceModelsAndManufacturers](../resources/manageddevicemodelsandmanufacturers.md)|Models and Manufactures meatadata for managed devices in the account|
|mdmEnrolledCount|Int32|The number of devices enrolled in MDM|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.managedDeviceOverview",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": "Integer",
  "mdmEnrolledCount": "Integer",
  "dualEnrolledDeviceCount": "Integer",
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.management.services.api.deviceOperatingSystemSummary"
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.management.services.api.deviceExchangeAccessStateSummary"
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.management.services.api.managedDeviceModelsAndManufacturers"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

