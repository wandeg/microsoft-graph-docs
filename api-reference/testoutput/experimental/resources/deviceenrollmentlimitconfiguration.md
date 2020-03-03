---
title: "deviceEnrollmentLimitConfiguration resource type"
description: "Device Enrollment Configuration that restricts the number of devices a user can enroll"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceEnrollmentLimitConfiguration resource type


Namespace: microsoft.graph

Device Enrollment Configuration that restricts the number of devices a user can enroll


Inherits from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceEnrollmentLimitConfigurations](../api/deviceenrollmentlimitconfiguration-list.md)|[deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md) collection|List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md) objects.|
|[Get deviceEnrollmentLimitConfiguration](../api/deviceenrollmentlimitconfiguration-get.md)|[deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md)|Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md) object.|
|[Create deviceEnrollmentLimitConfiguration](../api/deviceenrollmentlimitconfiguration-create.md)|[deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md)|Create a new [deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md) object.|
|[Delete deviceEnrollmentLimitConfiguration](../api/deviceenrollmentlimitconfiguration-delete.md)|None|Deletes a [deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md).|
|[Update deviceEnrollmentLimitConfiguration](../api/deviceenrollmentlimitconfiguration-update.md)|[deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md)|Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md) object.|
|[setPriority](../api/deviceenrollmentlimitconfiguration-setpriority.md)|None||
|[assign](../api/deviceenrollmentlimitconfiguration-assign.md)|None||
|[List assignments](../api/deviceenrollmentlimitconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|Get the enrollmentConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/deviceenrollmentlimitconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|description|String|The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|displayName|String|The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|limit|Int32|The maximum number of devices that a user can enroll|
|priority|Int32|Priority is used when a user exists in multiple groups that are assigned enrollment configuration. Users are subject only to the configuration with the lowest priority value. Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|version|Int32|The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentLimitConfiguration",
  "baseType": "microsoft.graph.deviceEnrollmentConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "limit": 1024
}
```

