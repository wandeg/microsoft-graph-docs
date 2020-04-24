---
title: "List autopilotEvents"
description: "Get the deviceManagementAutopilotEvents from the autopilotEvents navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List autopilotEvents

Namespace: microsoft.graph

Get the deviceManagementAutopilotEvents from the autopilotEvents navigation property.

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
GET /deviceManagement/autopilotEvents
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAutopilotEvent](../resources/devicemanagementautopilotevent.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementautopilotevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementautopilotevent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

