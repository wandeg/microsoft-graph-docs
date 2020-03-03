---
title: "Get remoteActionAudit"
description: "Read properties and relationships of the remoteActionAudit object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get remoteActionAudit

Namespace: microsoft.graph

Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.

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
GET /deviceManagement/remoteActionAudits/{remoteActionAuditId}
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
If successful, this method returns a `200 OK` response code and [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_remoteactionaudit"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 587

{
  "value": {
    "@odata.type": "#microsoft.graph.remoteActionAudit",
    "id": "d2d45e42-5e42-d2d4-425e-d4d2425ed4d2",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
    "action": "String",
    "requestDateTime": "2017-01-01T00:00:58.3860693+03:00",
    "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
    "deviceIMEI": "Device IMEI value",
    "actionState": "String",
    "managedDeviceId": "Managed Device Id value"
  }
}
```

