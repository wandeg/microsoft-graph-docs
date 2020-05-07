---
title: "deviceManagementAutopilotEvent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementAutopilotEvent resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List policyStatusDetails](../api/devicemanagementautopilotevent-list-policystatusdetails.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) collection|Get the deviceManagementAutopilotPolicyStatusDetails from the policyStatusDetails navigation property.|
|[Create policyStatusDetails](../api/devicemanagementautopilotevent-post-policystatusdetails.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md)|Create a new policyStatusDetails object.|
|[Delete policyStatusDetails](../api/devicemanagementautopilotevent-delete-policystatusdetails.md)|None|Delete a [deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) object.|
|[Update policyStatusDetails](../api/devicemanagementautopilotevent-update-policystatusdetails.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md)|Update the properties of a policyStatusDetails object.|
|[Get deviceManagementAutopilotPolicyStatusDetail](../api/devicemanagementautopilotpolicystatusdetail-get.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md)|Read the properties and relationships of a [deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountSetupDuration|Duration|**TODO: Add Description**|
|deploymentDuration|Duration|**TODO: Add Description**|
|deploymentEndDateTime|DateTimeOffset|**TODO: Add Description**|
|deploymentStartDateTime|DateTimeOffset|**TODO: Add Description**|
|deploymentState|windowsAutopilotDeploymentState|**TODO: Add Description**. Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.|
|deploymentTotalDuration|Duration|**TODO: Add Description**|
|deviceId|String|**TODO: Add Description**|
|devicePreparationDuration|Duration|**TODO: Add Description**|
|deviceRegisteredDateTime|DateTimeOffset|**TODO: Add Description**|
|deviceSerialNumber|String|**TODO: Add Description**|
|deviceSetupDuration|Duration|**TODO: Add Description**|
|enrollmentFailureDetails|String|**TODO: Add Description**|
|enrollmentStartDateTime|DateTimeOffset|**TODO: Add Description**|
|enrollmentState|enrollmentState|**TODO: Add Description**. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|enrollmentType|windowsAutopilotEnrollmentType|**TODO: Add Description**. Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|eventDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|managedDeviceName|String|**TODO: Add Description**|
|osVersion|String|**TODO: Add Description**|
|targetedAppCount|Int32|**TODO: Add Description**|
|targetedPolicyCount|Int32|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|windows10EnrollmentCompletionPageConfigurationDisplayName|String|**TODO: Add Description**|
|windowsAutopilotDeploymentProfileDisplayName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|policyStatusDetails|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "targetedAppCount": "Integer",
  "targetedPolicyCount": "Integer",
  "enrollmentFailureDetails": "String"
}
```

