---
title: "Create deviceManagementAutopilotEvent"
description: "Create a new deviceManagementAutopilotEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create deviceManagementAutopilotEvent

Namespace: microsoft.graph

Create a new [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.

The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|eventDateTime|DateTimeOffset|Time when the event occurred .|
|deviceRegisteredDateTime|DateTimeOffset|Device registration date.|
|enrollmentStartDateTime|DateTimeOffset|Device enrollment start date.|
|enrollmentType|Enumeration|Enrollment type. Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|deviceSerialNumber|String|Device serial number.|
|managedDeviceName|String|Managed device name.|
|userPrincipalName|String|User principal name used to enroll the device.|
|windowsAutopilotDeploymentProfileDisplayName|String|Autopilot profile name.|
|enrollmentState|Enumeration|Enrollment state like Enrolled, Failed. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|String|Enrollment Status Page profile name|
|deploymentState|Enumeration|Deployment state like Success, Failure, InProgress, SuccessWithTimeout. Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.|
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

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementautopilotevent_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1288

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "eventDateTime": "2017-01-01T00:01:42.7768776+03:00",
  "deviceRegisteredDateTime": "2016-12-31T23:57:58.8773333+03:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:10.1686596+03:00",
  "enrollmentType": "String",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "String",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "String",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT29.5064364S",
  "deploymentTotalDuration": "PT1M12.7835476S",
  "devicePreparationDuration": "PT3M6.0815359S",
  "deviceSetupDuration": "-PT1M48.0144406S",
  "accountSetupDuration": "-PT2M58.717337S",
  "deploymentStartDateTime": "2017-01-01T00:02:30.5949761+03:00",
  "deploymentEndDateTime": "2017-01-01T00:02:33.572833+03:00",
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
Content-Length: 1337

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "4dbdd31d-d31d-4dbd-1dd3-bd4d1dd3bd4d",
  "eventDateTime": "2017-01-01T00:01:42.7768776+03:00",
  "deviceRegisteredDateTime": "2016-12-31T23:57:58.8773333+03:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:10.1686596+03:00",
  "enrollmentType": "String",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "String",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "String",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT29.5064364S",
  "deploymentTotalDuration": "PT1M12.7835476S",
  "devicePreparationDuration": "PT3M6.0815359S",
  "deviceSetupDuration": "-PT1M48.0144406S",
  "accountSetupDuration": "-PT2M58.717337S",
  "deploymentStartDateTime": "2017-01-01T00:02:30.5949761+03:00",
  "deploymentEndDateTime": "2017-01-01T00:02:33.572833+03:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```

