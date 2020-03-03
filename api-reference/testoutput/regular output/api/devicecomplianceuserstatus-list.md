---
title: "List deviceComplianceUserStatuses"
description: "List properties and relationships of the deviceComplianceUserStatus objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceComplianceUserStatuses

Namespace: microsoft.graph

List properties and relationships of the [deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) objects.

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
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicecomplianceuserstatus"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicecomplianceuserstatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 390

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
      "id": "02ae9416-9416-02ae-1694-ae021694ae02",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "String",
      "lastReportedDateTime": "2017-01-01T00:01:14.9975606+03:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```

