---
title: "Add autopilotEvents"
description: "Add autopilotEvents by posting to the autopilotEvents collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add autopilotEvents

Namespace: microsoft.graph

Add autopilotEvents by posting to the autopilotEvents collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.

The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deviceId|String||
|eventDateTime|DateTimeOffset||
|deviceRegisteredDateTime|DateTimeOffset||
|enrollmentStartDateTime|DateTimeOffset||
|enrollmentType|Enumeration| Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|deviceSerialNumber|String||
|managedDeviceName|String||
|userPrincipalName|String||
|windowsAutopilotDeploymentProfileDisplayName|String||
|enrollmentState|Enumeration| Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|String||
|deploymentState|Enumeration| Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.|
|osVersion|String||
|deploymentDuration|Duration||
|deploymentTotalDuration|Duration||
|devicePreparationDuration|Duration||
|deviceSetupDuration|Duration||
|accountSetupDuration|Duration||
|deploymentStartDateTime|DateTimeOffset||
|deploymentEndDateTime|DateTimeOffset||
|targetedAppCount|Int32||
|targetedPolicyCount|Int32||
|enrollmentFailureDetails|String||



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementautopilotevent_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1320

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "deviceId": "Device Id value",
  "eventDateTime": "2016-12-31T23:59:13.0497597+00:00",
  "deviceRegisteredDateTime": "2016-12-31T23:59:08.9900844+00:00",
  "enrollmentStartDateTime": "2016-12-31T23:56:51.6225999+00:00",
  "enrollmentType": "String",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "String",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "String",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT2M18.8544041S",
  "deploymentTotalDuration": "-PT35.9373414S",
  "devicePreparationDuration": "-PT3M29.9259289S",
  "deviceSetupDuration": "-PT44.239152S",
  "accountSetupDuration": "PT6.0687754S",
  "deploymentStartDateTime": "2016-12-31T23:56:52.1432186+00:00",
  "deploymentEndDateTime": "2016-12-31T23:58:32.6628304+00:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementautopilotevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1369

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "5f380702-0702-5f38-0207-385f0207385f",
  "deviceId": "Device Id value",
  "eventDateTime": "2016-12-31T23:59:13.0497597+00:00",
  "deviceRegisteredDateTime": "2016-12-31T23:59:08.9900844+00:00",
  "enrollmentStartDateTime": "2016-12-31T23:56:51.6225999+00:00",
  "enrollmentType": "String",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "String",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "String",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT2M18.8544041S",
  "deploymentTotalDuration": "-PT35.9373414S",
  "devicePreparationDuration": "-PT3M29.9259289S",
  "deviceSetupDuration": "-PT44.239152S",
  "accountSetupDuration": "PT6.0687754S",
  "deploymentStartDateTime": "2016-12-31T23:56:52.1432186+00:00",
  "deploymentEndDateTime": "2016-12-31T23:58:32.6628304+00:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```

