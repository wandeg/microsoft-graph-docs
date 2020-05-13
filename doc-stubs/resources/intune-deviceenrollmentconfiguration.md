---
title: "deviceEnrollmentConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceEnrollmentConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceEnrollmentConfigurations](../api/intune-devicemanagement-list-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md) collection|Get the deviceEnrollmentConfigurations from the deviceEnrollmentConfigurations navigation property.|
|[Create deviceEnrollmentConfigurations](../api/intune-devicemanagement-post-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md)|Create a new deviceEnrollmentConfigurations object.|
|[Delete deviceEnrollmentConfigurations](../api/intune-devicemanagement-delete-deviceenrollmentconfigurations.md)|None|Delete a [deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md) object.|
|[Update deviceEnrollmentConfigurations](../api/intune-devicemanagement-update-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md)|Update the properties of a deviceEnrollmentConfigurations object.|
|[Get deviceEnrollmentConfigurations](../api/intune-devicemanagement-get-deviceenrollmentconfiguration.md)|[deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md)|Read the properties and relationships of a [deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md) object.|
|[setPriority](../api/intune-deviceenrollmentconfiguration-setpriority.md)|None|**TODO: Add Description**|
|[assign](../api/intune-deviceenrollmentconfiguration-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/intune-deviceenrollmentconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md) collection|Get the enrollmentConfigurationAssignments from the assignments navigation property.|
|[Create assignments](../api/intune-deviceenrollmentconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/intune-deviceenrollmentconfiguration-delete-assignments.md)|None|Delete an [enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md) object.|
|[Update assignments](../api/intune-deviceenrollmentconfiguration-update-assignments.md)|[enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md)|Update the properties of an assignments object.|
|[Get assignments](../api/intune-deviceenrollmentconfiguration-get-enrollmentconfigurationassignment.md)|[enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md)|Read the properties and relationships of an [enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "priority": "Integer",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": "Integer"
}
```

