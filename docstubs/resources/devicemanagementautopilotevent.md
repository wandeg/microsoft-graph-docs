---
title: "deviceManagementAutopilotEvent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementAutopilotEvent resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementAutopilotEvent](../api/devicemanagementautopilotevent-get.md)|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md)|Read properties and relationships of the [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.|
|[Update deviceManagementAutopilotEvent](../api/devicemanagementautopilotevent-update.md)|[deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md)|Update the properties of a [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.|
|[List policyStatusDetails](../api/devicemanagementautopilotevent-list-policystatusdetails.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) collection|Get the deviceManagementAutopilotPolicyStatusDetails from the policyStatusDetails navigation property.|
|[Add policyStatusDetails](../api/devicemanagementautopilotevent-post-policystatusdetails.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md)|Add policyStatusDetails by posting to the policyStatusDetails collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountSetupDuration|Duration||
|deploymentDuration|Duration||
|deploymentEndDateTime|DateTimeOffset||
|deploymentStartDateTime|DateTimeOffset||
|deploymentState|Enumeration| Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.|
|deploymentTotalDuration|Duration||
|deviceId|String||
|devicePreparationDuration|Duration||
|deviceRegisteredDateTime|DateTimeOffset||
|deviceSerialNumber|String||
|deviceSetupDuration|Duration||
|enrollmentFailureDetails|String||
|enrollmentStartDateTime|DateTimeOffset||
|enrollmentState|Enumeration| Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|enrollmentType|Enumeration| Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|eventDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|managedDeviceName|String||
|osVersion|String||
|targetedAppCount|Int32||
|targetedPolicyCount|Int32||
|userPrincipalName|String||
|windows10EnrollmentCompletionPageConfigurationDisplayName|String||
|windowsAutopilotDeploymentProfileDisplayName|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|policyStatusDetails|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) collection||

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

