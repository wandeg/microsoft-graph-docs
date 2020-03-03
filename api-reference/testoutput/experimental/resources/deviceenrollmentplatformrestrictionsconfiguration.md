---
title: "deviceEnrollmentPlatformRestrictionsConfiguration resource type"
description: "Device Enrollment Configuration that restricts the types of devices a user can enroll"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceEnrollmentPlatformRestrictionsConfiguration resource type

Device Enrollment Configuration that restricts the types of devices a user can enroll


Inherits from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceEnrollmentPlatformRestrictionsConfigurations](../api/deviceenrollmentplatformrestrictionsconfiguration-list.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceEnrollmentPlatformRestrictionsConfiguration.md) collection|List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md) objects.|
|[Get deviceEnrollmentPlatformRestrictionsConfiguration](../api/deviceenrollmentplatformrestrictionsconfiguration-get.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceEnrollmentPlatformRestrictionsConfiguration.md)|Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md) object.|
|[Create deviceEnrollmentPlatformRestrictionsConfiguration](../api/deviceenrollmentplatformrestrictionsconfiguration-create.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceEnrollmentPlatformRestrictionsConfiguration.md)|Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md) object.|
|[Delete deviceEnrollmentPlatformRestrictionsConfiguration](../api/deviceenrollmentplatformrestrictionsconfiguration-delete.md)|None|Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md).|
|[Update deviceEnrollmentPlatformRestrictionsConfiguration](../api/deviceenrollmentplatformrestrictionsconfiguration-update.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceEnrollmentPlatformRestrictionsConfiguration.md)|Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md) object.|
|[setPriority](../api/deviceenrollmentplatformrestrictionsconfiguration-setpriority.md)|None||
|[assign](../api/deviceenrollmentplatformrestrictionsconfiguration-assign.md)|None||
|[List assignments](../api/deviceenrollmentplatformrestrictionsconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentConfigurationAssignment.md) collection|Get the enrollmentConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/deviceenrollmentplatformrestrictionsconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidForWorkRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceEnrollmentPlatformRestriction.md)|Android for work restrictions based on platform, platform operating system version, and device ownership|
|androidRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceEnrollmentPlatformRestriction.md)|Android restrictions based on platform, platform operating system version, and device ownership|
|createdDateTime|DateTimeOffset|Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|description|String|The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|displayName|String|The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|iosRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceEnrollmentPlatformRestriction.md)|Ios restrictions based on platform, platform operating system version, and device ownership|
|lastModifiedDateTime|DateTimeOffset|Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|macOSRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceEnrollmentPlatformRestriction.md)|Mac restrictions based on platform, platform operating system version, and device ownership|
|macRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceEnrollmentPlatformRestriction.md)|Mac restrictions based on platform, platform operating system version, and device ownership|
|priority|Int32|Priority is used when a user exists in multiple groups that are assigned enrollment configuration. Users are subject only to the configuration with the lowest priority value. Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|version|Int32|The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|windowsMobileRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceEnrollmentPlatformRestriction.md)|Windows mobile restrictions based on platform, platform operating system version, and device ownership|
|windowsRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceEnrollmentPlatformRestriction.md)|Windows restrictions based on platform, platform operating system version, and device ownership|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/enrollmentConfigurationAssignment.md) collection|The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "baseType": "microsoft.graph.deviceEnrollmentConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
  }
}
```

