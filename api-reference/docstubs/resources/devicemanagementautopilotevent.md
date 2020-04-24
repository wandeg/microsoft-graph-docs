---
title: "deviceManagementAutopilotEvent resource type"
description: "Represents an Autopilot flow event."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementAutopilotEvent resource type


Namespace: microsoft.graph

Represents an Autopilot flow event.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementAutopilotEvent](../api/devicemanagementautopilotevent-get.md)|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md)|Read the properties and relationships of a [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.|
|[Update deviceManagementAutopilotEvent](../api/devicemanagementautopilotevent-update.md)|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md)|Update the properties of a [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.|
|[List policyStatusDetails](../api/devicemanagementautopilotevent-list-policystatusdetails.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) collection|Get the deviceManagementAutopilotPolicyStatusDetails from the policyStatusDetails navigation property.|
|[Create policyStatusDetails](../api/devicemanagementautopilotevent-post-policystatusdetails.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md)|Create a new policyStatusDetails object.|
|[Delete policyStatusDetails](../api/devicemanagementautopilotevent-delete-policystatusdetails.md)|None|Delete a [deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) object.|
|[Update policyStatusDetails](../api/devicemanagementautopilotevent-update-policystatusdetails.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md)|Update the properties of a policyStatusDetails object.|
|[Get deviceManagementAutopilotPolicyStatusDetail](../api/devicemanagementautopilotpolicystatusdetail-get.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md)|Read the properties and relationships of a [deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountSetupDuration|Duration|Time spent in user ESP.|
|deploymentDuration|Duration|Autopilot deployment duration including enrollment.|
|deploymentEndDateTime|DateTimeOffset|Deployment end time.|
|deploymentStartDateTime|DateTimeOffset|Deployment start time.|
|deploymentState|windowsAutopilotDeploymentState|Deployment state like Success, Failure, InProgress, SuccessWithTimeout. Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.|
|deploymentTotalDuration|Duration|Total deployment duration from enrollment to Desktop screen.|
|deviceId|String|Device id associated with the object|
|devicePreparationDuration|Duration|Time spent in device enrollment.|
|deviceRegisteredDateTime|DateTimeOffset|Device registration date.|
|deviceSerialNumber|String|Device serial number.|
|deviceSetupDuration|Duration|Time spent in device ESP.|
|enrollmentFailureDetails|String|Enrollment failure details.|
|enrollmentStartDateTime|DateTimeOffset|Device enrollment start date.|
|enrollmentState|enrollmentState|Enrollment state like Enrolled, Failed. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|enrollmentType|windowsAutopilotEnrollmentType|Enrollment type. Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|eventDateTime|DateTimeOffset|Time when the event occurred .|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|managedDeviceName|String|Managed device name.|
|osVersion|String|Device operating system version.|
|targetedAppCount|Int32|Count of applications targeted.|
|targetedPolicyCount|Int32|Count of policies targeted.|
|userPrincipalName|String|User principal name used to enroll the device.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|String|Enrollment Status Page profile name|
|windowsAutopilotDeploymentProfileDisplayName|String|Autopilot profile name.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|policyStatusDetails|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) collection|Policy and application status details for this device.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAutopilotEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "String (identifier)",
  "deviceId": "String",
  "eventDateTime": "String (timestamp)",
  "deviceRegisteredDateTime": "String (timestamp)",
  "enrollmentStartDateTime": "String (timestamp)",
  "enrollmentType": "String",
  "deviceSerialNumber": "String",
  "managedDeviceName": "String",
  "userPrincipalName": "String",
  "windowsAutopilotDeploymentProfileDisplayName": "String",
  "enrollmentState": "String",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "String",
  "deploymentState": "String",
  "osVersion": "String",
  "deploymentDuration": "String (duration)",
  "deploymentTotalDuration": "String (duration)",
  "devicePreparationDuration": "String (duration)",
  "deviceSetupDuration": "String (duration)",
  "accountSetupDuration": "String (duration)",
  "deploymentStartDateTime": "String (timestamp)",
  "deploymentEndDateTime": "String (timestamp)",
  "targetedAppCount": 1024,
  "targetedPolicyCount": 1024,
  "enrollmentFailureDetails": "String"
}
```

