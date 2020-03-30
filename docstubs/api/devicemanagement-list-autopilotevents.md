---
title: "List autopilotEvents"
description: "Get the deviceManagementAutopilotEvents from the autopilotEvents navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List autopilotEvents

Namespace: microsoft.graph

Get the deviceManagementAutopilotEvents from the autopilotEvents navigation property.

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
GET /deviceManagement/autopilotEvents
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
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementautopilotevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
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
Content-Length: 1507

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
      "id": "a7159688-9688-a715-8896-15a7889615a7",
      "deviceId": "Device Id value",
      "eventDateTime": "2017-01-01T00:02:22.1549518+03:00",
      "deviceRegisteredDateTime": "2016-12-31T23:56:33.198831+03:00",
      "enrollmentStartDateTime": "2017-01-01T00:01:28.4079818+03:00",
      "enrollmentType": "String",
      "deviceSerialNumber": "Device Serial Number value",
      "managedDeviceName": "Managed Device Name value",
      "userPrincipalName": "User Principal Name value",
      "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
      "enrollmentState": "String",
      "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
      "deploymentState": "String",
      "osVersion": "Os Version value",
      "deploymentDuration": "PT2M29.4111152S",
      "deploymentTotalDuration": "-PT53.4684442S",
      "devicePreparationDuration": "PT3M10.2146348S",
      "deviceSetupDuration": "-PT3M31.6961771S",
      "accountSetupDuration": "-PT1M55.4973674S",
      "deploymentStartDateTime": "2016-12-31T23:59:17.0730357+03:00",
      "deploymentEndDateTime": "2017-01-01T00:02:48.9829296+03:00",
      "targetedAppCount": 0,
      "targetedPolicyCount": 3,
      "enrollmentFailureDetails": "Enrollment Failure Details value"
    }
  ]
}
```

