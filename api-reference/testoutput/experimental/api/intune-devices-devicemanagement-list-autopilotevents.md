---
title: "List autopilotEvents"
description: "Get the deviceManagementAutopilotEvents from the autopilotEvents navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List autopilotEvents

Get the deviceManagementAutopilotEvents from the autopilotEvents navigation property.

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
GET /deviceManagement/autopilotEvents
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementautopilotevent"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/deviceManagement/autopilotEvents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementautopilotevent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1465

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
      "id": "47a0d7cd-d7cd-47a0-cdd7-a047cdd7a047",
      "eventDateTime": "2017-01-01T00:00:02.9716266+03:00",
      "deviceRegisteredDateTime": "2016-12-31T23:56:35.5014109+03:00",
      "enrollmentStartDateTime": "2017-01-01T00:01:38.6767976+03:00",
      "enrollmentType": "String",
      "deviceSerialNumber": "Device Serial Number value",
      "managedDeviceName": "Managed Device Name value",
      "userPrincipalName": "User Principal Name value",
      "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
      "enrollmentState": "String",
      "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
      "deploymentState": "String",
      "osVersion": "Os Version value",
      "deploymentDuration": "PT1M19.8993895S",
      "deploymentTotalDuration": "-PT26.7870562S",
      "devicePreparationDuration": "-PT2M54.2816142S",
      "deviceSetupDuration": "-PT19.358251S",
      "accountSetupDuration": "PT51.8649448S",
      "deploymentStartDateTime": "2016-12-31T23:58:32.8953409+03:00",
      "deploymentEndDateTime": "2016-12-31T23:59:33.4308442+03:00",
      "targetedAppCount": 0,
      "targetedPolicyCount": 3,
      "enrollmentFailureDetails": "Enrollment Failure Details value"
    }
  ]
}
```

