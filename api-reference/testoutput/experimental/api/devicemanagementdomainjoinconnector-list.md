---
title: "List deviceManagementDomainJoinConnectors"
description: "List properties and relationships of the deviceManagementDomainJoinConnector objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceManagementDomainJoinConnectors

Namespace: microsoft.graph

List properties and relationships of the [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) objects.

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
GET /deviceManagement/domainJoinConnectors
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementdomainjoinconnector"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/domainJoinConnectors
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementdomainjoinconnector)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
      "id": "a924df48-df48-a924-48df-24a948df24a9",
      "displayName": "Display Name value",
      "lastConnectionDateTime": "2016-12-31T23:56:25.4273633+03:00",
      "state": "String",
      "version": "Version value"
    }
  ]
}
```

