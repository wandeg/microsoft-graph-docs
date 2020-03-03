---
title: "windows10EnrollmentCompletionPageConfiguration resource type"
description: "Windows 10 Enrollment Status Page Configuration"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windows10EnrollmentCompletionPageConfiguration resource type


Namespace: microsoft.graph

Windows 10 Enrollment Status Page Configuration


Inherits from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windows10EnrollmentCompletionPageConfigurations](../api/windows10enrollmentcompletionpageconfiguration-list.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/windows10enrollmentcompletionpageconfiguration.md) collection|List properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/windows10enrollmentcompletionpageconfiguration.md) objects.|
|[Get windows10EnrollmentCompletionPageConfiguration](../api/windows10enrollmentcompletionpageconfiguration-get.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/windows10enrollmentcompletionpageconfiguration.md)|Read properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/windows10enrollmentcompletionpageconfiguration.md) object.|
|[Create windows10EnrollmentCompletionPageConfiguration](../api/windows10enrollmentcompletionpageconfiguration-create.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/windows10enrollmentcompletionpageconfiguration.md)|Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/windows10enrollmentcompletionpageconfiguration.md) object.|
|[Delete windows10EnrollmentCompletionPageConfiguration](../api/windows10enrollmentcompletionpageconfiguration-delete.md)|None|Deletes a [windows10EnrollmentCompletionPageConfiguration](../resources/windows10enrollmentcompletionpageconfiguration.md).|
|[Update windows10EnrollmentCompletionPageConfiguration](../api/windows10enrollmentcompletionpageconfiguration-update.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/windows10enrollmentcompletionpageconfiguration.md)|Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/windows10enrollmentcompletionpageconfiguration.md) object.|
|[setPriority](../api/windows10enrollmentcompletionpageconfiguration-setpriority.md)|None||
|[assign](../api/windows10enrollmentcompletionpageconfiguration-assign.md)|None||
|[List assignments](../api/windows10enrollmentcompletionpageconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|Get the enrollmentConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/windows10enrollmentcompletionpageconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowDeviceResetOnInstallFailure|Boolean|Allow or block device reset on installation failure|
|allowDeviceUseOnInstallFailure|Boolean|Allow the user to continue using the device on installation failure|
|allowLogCollectionOnInstallFailure|Boolean|Allow or block log collection on installation failure|
|blockDeviceSetupRetryByUser|Boolean|Allow the user to retry the setup on installation failure|
|createdDateTime|DateTimeOffset|Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|customErrorMessage|String|Set custom error message to show upon installation failure|
|description|String|The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|disableUserStatusTrackingAfterFirstUser|Boolean|Only show installation progress for first user post enrollment|
|displayName|String|The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|installProgressTimeoutInMinutes|Int32|Set installation progress timeout in minutes|
|lastModifiedDateTime|DateTimeOffset|Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|priority|Int32|Priority is used when a user exists in multiple groups that are assigned enrollment configuration. Users are subject only to the configuration with the lowest priority value. Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|selectedMobileAppIds|String collection|Selected applications to track the installation status|
|showInstallationProgress|Boolean|Show or hide installation progress to user|
|trackInstallProgressForAutopilotOnly|Boolean|Only show installation progress for Autopilot enrollment scenarios|
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
  "@odata.type": "microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "baseType": "microsoft.graph.deviceEnrollmentConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "String"
  ],
  "trackInstallProgressForAutopilotOnly": true,
  "disableUserStatusTrackingAfterFirstUser": true
}
```

