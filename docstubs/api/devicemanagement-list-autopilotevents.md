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
      "id": "524ad46a-d46a-524a-6ad4-4a526ad44a52",
      "deviceId": "Device Id value",
      "eventDateTime": "2017-01-01T00:00:27.7992878+03:00",
      "deviceRegisteredDateTime": "2017-01-01T00:03:13.2647535+03:00",
      "enrollmentStartDateTime": "2017-01-01T00:01:37.6593112+03:00",
      "enrollmentType": "String",
      "deviceSerialNumber": "Device Serial Number value",
      "managedDeviceName": "Managed Device Name value",
      "userPrincipalName": "User Principal Name value",
      "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
      "enrollmentState": "String",
      "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
      "deploymentState": "String",
      "osVersion": "Os Version value",
      "deploymentDuration": "-PT46.5939702S",
      "deploymentTotalDuration": "-PT2M44.4109596S",
      "devicePreparationDuration": "-PT42.7195922S",
      "deviceSetupDuration": "PT3M31.4050478S",
      "accountSetupDuration": "-PT1M56.2952771S",
      "deploymentStartDateTime": "2017-01-01T00:02:38.8090363+03:00",
      "deploymentEndDateTime": "2017-01-01T00:00:40.2623288+03:00",
      "targetedAppCount": 0,
      "targetedPolicyCount": 3,
      "enrollmentFailureDetails": "Enrollment Failure Details value"
    }
  ]
}
```

