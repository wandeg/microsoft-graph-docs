---
title: "deviceEnrollmentPlatformRestrictionsConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceEnrollmentPlatformRestrictionsConfiguration resource type


Namespace: microsoft.graph




Inherits from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceEnrollmentPlatformRestrictionsConfigurations](../api/deviceenrollmentplatformrestrictionsconfiguration-list.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md) collection|List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md) objects.|
|[Get deviceEnrollmentPlatformRestrictionsConfiguration](../api/deviceenrollmentplatformrestrictionsconfiguration-get.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md)|Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md) object.|
|[Create deviceEnrollmentPlatformRestrictionsConfiguration](../api/deviceenrollmentplatformrestrictionsconfiguration-create.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md)|Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md) object.|
|[Delete deviceEnrollmentPlatformRestrictionsConfiguration](../api/deviceenrollmentplatformrestrictionsconfiguration-delete.md)|None|Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md).|
|[Update deviceEnrollmentPlatformRestrictionsConfiguration](../api/deviceenrollmentplatformrestrictionsconfiguration-update.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md)|Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/deviceenrollmentplatformrestrictionsconfiguration.md) object.|
|[setPriority](../api/deviceenrollmentplatformrestrictionsconfiguration-setpriority.md)|None||
|[assign](../api/deviceenrollmentplatformrestrictionsconfiguration-assign.md)|None||
|[List assignments](../api/deviceenrollmentplatformrestrictionsconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|Get the enrollmentConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/deviceenrollmentplatformrestrictionsconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceenrollmentplatformrestriction.md)||
|createdDateTime|DateTimeOffset| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|description|String| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|displayName|String| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|iosRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceenrollmentplatformrestriction.md)||
|lastModifiedDateTime|DateTimeOffset| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|macOSRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceenrollmentplatformrestriction.md)||
|priority|Int32| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|version|Int32| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|windowsMobileRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceenrollmentplatformrestriction.md)||
|windowsRestriction|[deviceEnrollmentPlatformRestriction](../resources/deviceenrollmentplatformrestriction.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|

## JSON representation
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
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
  }
}
```

