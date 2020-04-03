---
title: "Get deviceManagementAutopilotPolicyStatusDetail"
description: "Read properties and relationships of the deviceManagementAutopilotPolicyStatusDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceManagementAutopilotPolicyStatusDetail

Namespace: microsoft.graph

Read properties and relationships of the [deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) object.

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
GET /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
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
If successful, this method returns a `200 OK` response code and [deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementautopilotpolicystatusdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementAutopilotPolicyStatusDetail"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 369

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
    "id": "679bd62f-d62f-679b-2fd6-9b672fd69b67",
    "displayName": "Display Name value",
    "policyType": "String",
    "complianceStatus": "String",
    "trackedOnEnrollmentStatus": true,
    "lastReportedDateTime": "2016-12-31T23:57:45.8617849+00:00"
  }
}
```

