---
title: "List deviceStatuses"
description: "Get the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatuses from the deviceStatuses navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceStatuses

Namespace: microsoft.graph

Get the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatuses from the deviceStatuses navigation property.

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
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
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
If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
      "id": "8b14c220-c220-8b14-20c2-148b20c2148b",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:02:12.9318449+03:00",
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "deploymentStatus": "String",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "policyVersion": "Policy Version value"
    }
  ]
}
```

