---
title: "deviceEnrollmentConfiguration resource type"
description: "The Base Class of Device Enrollment Configuration"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceEnrollmentConfiguration resource type


Namespace: microsoft.graph

The Base Class of Device Enrollment Configuration


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceEnrollmentConfiguration](../api/deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|Read the properties and relationships of a [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) object.|
|[hasPayloadLinks](../api/deviceenrollmentconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection|**TODO: Add Description**|
|[setPriority](../api/deviceenrollmentconfiguration-setpriority.md)|None|**TODO: Add Description**|
|[assign](../api/deviceenrollmentconfiguration-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/deviceenrollmentconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|Get the enrollmentConfigurationAssignments from the assignments navigation property.|
|[Create assignments](../api/deviceenrollmentconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/deviceenrollmentconfiguration-delete-assignments.md)|None|Delete an [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) object.|
|[Update assignments](../api/deviceenrollmentconfiguration-update-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Update the properties of an assignments object.|
|[Get enrollmentConfigurationAssignment](../api/enrollmentconfigurationassignment-get.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Read the properties and relationships of an [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) object.|
|[List deviceEnrollmentConfigurations](../api/user-list-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) collection|Get the deviceEnrollmentConfigurations from the deviceEnrollmentConfigurations navigation property.|
|[Create deviceEnrollmentConfigurations](../api/user-post-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|Create a new deviceEnrollmentConfigurations object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Created date time in UTC of the device enrollment configuration|
|description|String|The description of the device enrollment configuration|
|displayName|String|The display name of the device enrollment configuration|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified date time in UTC of the device enrollment configuration|
|priority|Int32|Priority is used when a user exists in multiple groups that are assigned enrollment configuration. Users are subject only to the configuration with the lowest priority value.|
|version|Int32|The version of the device enrollment configuration|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|The list of group assignments for the device configuration profile|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```

