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

Read properties and relationships of the [remoteActionAudit](../resources/remoteactionaudit.md) object.

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
GET /deviceManagement/remoteActionAudits/{remoteActionAuditId}
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
If successful, this method returns a `200 OK` response code and [remoteActionAudit](../resources/remoteactionaudit.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_remoteactionaudit"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
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
    "id": "e67e4333-4333-e67e-3343-7ee633437ee6",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
    "action": "String",
    "requestDateTime": "2016-12-31T23:59:32.6730308+00:00",
    "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
    "deviceIMEI": "Device IMEI value",
    "actionState": "String",
    "managedDeviceId": "Managed Device Id value"
  }
}
```

