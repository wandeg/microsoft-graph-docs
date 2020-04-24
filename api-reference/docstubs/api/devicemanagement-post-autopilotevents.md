---
title: "Create autopilotEvents"
description: "Create a new autopilotEvents object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create autopilotEvents

Namespace: microsoft.graph

Create a new autopilotEvents object.

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
POST /deviceManagement/autopilotEvents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.

The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deviceId|String|Device id associated with the object|
|eventDateTime|DateTimeOffset|Time when the event occurred .|
|deviceRegisteredDateTime|DateTimeOffset|Device registration date.|
|enrollmentStartDateTime|DateTimeOffset|Device enrollment start date.|
|enrollmentType|windowsAutopilotEnrollmentType|Enrollment type. Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|deviceSerialNumber|String|Device serial number.|
|managedDeviceName|String|Managed device name.|
|userPrincipalName|String|User principal name used to enroll the device.|
|windowsAutopilotDeploymentProfileDisplayName|String|Autopilot profile name.|
|enrollmentState|enrollmentState|Enrollment state like Enrolled, Failed. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|String|Enrollment Status Page profile name|
|deploymentState|windowsAutopilotDeploymentState|Deployment state like Success, Failure, InProgress, SuccessWithTimeout. Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.|
|osVersion|String|Device operating system version.|
|deploymentDuration|Duration|Autopilot deployment duration including enrollment.|
|deploymentTotalDuration|Duration|Total deployment duration from enrollment to Desktop screen.|
|devicePreparationDuration|Duration|Time spent in device enrollment.|
|deviceSetupDuration|Duration|Time spent in device ESP.|
|accountSetupDuration|Duration|Time spent in user ESP.|
|deploymentStartDateTime|DateTimeOffset|Deployment start time.|
|deploymentEndDateTime|DateTimeOffset|Deployment end time.|
|targetedAppCount|Int32|Count of applications targeted.|
|targetedPolicyCount|Int32|Count of policies targeted.|
|enrollmentFailureDetails|String|Enrollment failure details.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementautopilotevent_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
Content-Type: application/json
Content-length: 1319

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "deviceId": "Device Id value",
  "eventDateTime": "2016-12-31T23:57:46.848839+03:00",
  "deviceRegisteredDateTime": "2016-12-31T23:59:07.389283+03:00",
  "enrollmentStartDateTime": "2017-01-01T00:01:12.0966565+03:00",
  "enrollmentType": "String",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "String",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "String",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT42.5735044S",
  "deploymentTotalDuration": "PT1M26.3527611S",
  "devicePreparationDuration": "PT2M36.587731S",
  "deviceSetupDuration": "PT2M0.6012241S",
  "accountSetupDuration": "PT1M59.5873672S",
  "deploymentStartDateTime": "2017-01-01T00:00:00.8427863+03:00",
  "deploymentEndDateTime": "2017-01-01T00:00:27.2069657+03:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementautopilotevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "e1150a41-0a41-e115-410a-15e1410a15e1",
  "deviceId": "Device Id value",
  "eventDateTime": "2016-12-31T23:57:46.848839+03:00",
  "deviceRegisteredDateTime": "2016-12-31T23:59:07.389283+03:00",
  "enrollmentStartDateTime": "2017-01-01T00:01:12.0966565+03:00",
  "enrollmentType": "String",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "String",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "String",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT42.5735044S",
  "deploymentTotalDuration": "PT1M26.3527611S",
  "devicePreparationDuration": "PT2M36.587731S",
  "deviceSetupDuration": "PT2M0.6012241S",
  "accountSetupDuration": "PT1M59.5873672S",
  "deploymentStartDateTime": "2017-01-01T00:00:00.8427863+03:00",
  "deploymentEndDateTime": "2017-01-01T00:00:27.2069657+03:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```

