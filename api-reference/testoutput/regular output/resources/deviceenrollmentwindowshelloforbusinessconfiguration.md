---
title: "deviceEnrollmentWindowsHelloForBusinessConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceEnrollmentWindowsHelloForBusinessConfiguration resource type


Namespace: microsoft.graph




Inherits from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceEnrollmentWindowsHelloForBusinessConfigurations](../api/deviceenrollmentwindowshelloforbusinessconfiguration-list.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) collection|List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.|
|[Get deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/deviceenrollmentwindowshelloforbusinessconfiguration-get.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md)|Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) object.|
|[Create deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/deviceenrollmentwindowshelloforbusinessconfiguration-create.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md)|Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) object.|
|[Delete deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/deviceenrollmentwindowshelloforbusinessconfiguration-delete.md)|None|Deletes a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Update deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/deviceenrollmentwindowshelloforbusinessconfiguration-update.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md)|Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) object.|
|[setPriority](../api/deviceenrollmentwindowshelloforbusinessconfiguration-setpriority.md)|None||
|[assign](../api/deviceenrollmentwindowshelloforbusinessconfiguration-assign.md)|None||
|[List assignments](../api/deviceenrollmentwindowshelloforbusinessconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|Get the enrollmentConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/deviceenrollmentwindowshelloforbusinessconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|description|String| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|displayName|String| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|enhancedBiometricsState|Enumeration|. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|pinExpirationInDays|Int32||
|pinLowercaseCharactersUsage|Enumeration|. Possible values are: `allowed`, `required`, `disallowed`.|
|pinMaximumLength|Int32||
|pinMinimumLength|Int32||
|pinPreviousBlockCount|Int32||
|pinSpecialCharactersUsage|Enumeration|. Possible values are: `allowed`, `required`, `disallowed`.|
|pinUppercaseCharactersUsage|Enumeration|. Possible values are: `allowed`, `required`, `disallowed`.|
|priority|Int32| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|remotePassportEnabled|Boolean||
|securityDeviceRequired|Boolean||
|state|Enumeration|. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|unlockWithBiometricsEnabled|Boolean||
|version|Int32| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "baseType": "microsoft.graph.deviceEnrollmentConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "state": "String",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 1024,
  "pinExpirationInDays": 1024,
  "enhancedBiometricsState": "String"
}
```

