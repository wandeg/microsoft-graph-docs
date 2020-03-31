---
title: "Get deviceManagementAutopilotEvent"
description: "Read properties and relationships of the deviceManagementAutopilotEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceManagementAutopilotEvent

Namespace: microsoft.graph

Read properties and relationships of the [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object.

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
GET /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementautopilotevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementAutopilotEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1444

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
    "id": "99d3562f-562f-99d3-2f56-d3992f56d399",
    "deviceId": "Device Id value",
    "eventDateTime": "2017-01-01T00:00:08.9877415+03:00",
    "deviceRegisteredDateTime": "2016-12-31T23:57:16.9725757+03:00",
    "enrollmentStartDateTime": "2016-12-31T23:59:49.824366+03:00",
    "enrollmentType": "String",
    "deviceSerialNumber": "Device Serial Number value",
    "managedDeviceName": "Managed Device Name value",
    "userPrincipalName": "User Principal Name value",
    "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
    "enrollmentState": "String",
    "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
    "deploymentState": "String",
    "osVersion": "Os Version value",
    "deploymentDuration": "PT1M57.0449049S",
    "deploymentTotalDuration": "-PT1M37.560664S",
    "devicePreparationDuration": "-PT1M38.7158703S",
    "deviceSetupDuration": "-PT1M1.6220064S",
    "accountSetupDuration": "-PT3M23.3085157S",
    "deploymentStartDateTime": "2017-01-01T00:01:31.6837201+03:00",
    "deploymentEndDateTime": "2016-12-31T23:57:16.3134655+03:00",
    "targetedAppCount": 0,
    "targetedPolicyCount": 3,
    "enrollmentFailureDetails": "Enrollment Failure Details value"
  }
}
```

