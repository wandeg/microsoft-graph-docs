---
title: "Update autopilotEvents"
description: "Update the properties of an autopilotEvents object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update autopilotEvents

Namespace: microsoft.graph

Update the properties of an autopilotEvents object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.

The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deviceId|String|**TODO: Add Description**|
|eventDateTime|DateTimeOffset|**TODO: Add Description**|
|deviceRegisteredDateTime|DateTimeOffset|**TODO: Add Description**|
|enrollmentStartDateTime|DateTimeOffset|**TODO: Add Description**|
|enrollmentType|windowsAutopilotEnrollmentType|**TODO: Add Description**. Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|deviceSerialNumber|String|**TODO: Add Description**|
|managedDeviceName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|windowsAutopilotDeploymentProfileDisplayName|String|**TODO: Add Description**|
|enrollmentState|enrollmentState|**TODO: Add Description**. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|String|**TODO: Add Description**|
|deploymentState|windowsAutopilotDeploymentState|**TODO: Add Description**. Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.|
|osVersion|String|**TODO: Add Description**|
|deploymentDuration|Duration|**TODO: Add Description**|
|deploymentTotalDuration|Duration|**TODO: Add Description**|
|devicePreparationDuration|Duration|**TODO: Add Description**|
|deviceSetupDuration|Duration|**TODO: Add Description**|
|accountSetupDuration|Duration|**TODO: Add Description**|
|deploymentStartDateTime|DateTimeOffset|**TODO: Add Description**|
|deploymentEndDateTime|DateTimeOffset|**TODO: Add Description**|
|targetedAppCount|Int32|**TODO: Add Description**|
|targetedPolicyCount|Int32|**TODO: Add Description**|
|enrollmentFailureDetails|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_autopilotevents"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
Content-Type: application/json
Content-length: 1062

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
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

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "b39e9087-9087-b39e-8790-9eb387909eb3",
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

