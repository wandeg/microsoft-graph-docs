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

## HTTP Request
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
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementautopilotevent"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
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
Content-Length: 1404

{
  "value": {
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
}
```

