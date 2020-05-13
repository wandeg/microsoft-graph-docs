---
title: "deviceEnrollmentPlatformRestrictionsConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceEnrollmentPlatformRestrictionsConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[setPriority](../api/intune-deviceenrollmentplatformrestrictionsconfiguration-setpriority.md)|None|**TODO: Add Description**|
|[assign](../api/intune-deviceenrollmentplatformrestrictionsconfiguration-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/intune-deviceenrollmentplatformrestrictionsconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md) collection|Get the enrollmentConfigurationAssignments from the assignments navigation property.|
|[Create assignments](../api/intune-deviceenrollmentplatformrestrictionsconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/intune-deviceenrollmentplatformrestrictionsconfiguration-delete-assignments.md)|None|Delete an [enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md) object.|
|[Update assignments](../api/intune-deviceenrollmentplatformrestrictionsconfiguration-update-assignments.md)|[enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md)|Update the properties of an assignments object.|
|[Get assignments](../api/intune-deviceenrollmentplatformrestrictionsconfiguration-get-enrollmentconfigurationassignment.md)|[enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md)|Read the properties and relationships of an [enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-deviceenrollmentplatformrestriction.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md)|
|description|String|**TODO: Add Description** Inherited from [deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md)|
|displayName|String|**TODO: Add Description** Inherited from [deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|iosRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-deviceenrollmentplatformrestriction.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md)|
|macOSRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-deviceenrollmentplatformrestriction.md)|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description** Inherited from [deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md)|
|version|Int32|**TODO: Add Description** Inherited from [deviceEnrollmentConfiguration](../resources/intune-deviceenrollmentconfiguration.md)|
|windowsMobileRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-deviceenrollmentplatformrestriction.md)|**TODO: Add Description**|
|windowsRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-deviceenrollmentplatformrestriction.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-enrollmentconfigurationassignment.md) collection|**TODO: Add Description** Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|

## JSON representation
The following is a JSON representation of the resource.
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
  "priority": "Integer",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": "Integer",
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
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

