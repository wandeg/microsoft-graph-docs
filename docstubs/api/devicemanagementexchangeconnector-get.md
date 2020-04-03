---
title: "Get deviceManagementExchangeConnector"
description: "Read properties and relationships of the deviceManagementExchangeConnector object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceManagementExchangeConnector

Namespace: microsoft.graph

Read properties and relationships of the [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object.

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
GET /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
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
If successful, this method returns a `200 OK` response code and [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementexchangeconnector"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementExchangeConnector"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 569

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
    "id": "0e31abb3-abb3-0e31-b3ab-310eb3ab310e",
    "lastSyncDateTime": "2016-12-31T23:57:21.5163223+00:00",
    "status": "String",
    "primarySmtpAddress": "Primary Smtp Address value",
    "serverName": "Server Name value",
    "connectorServerName": "Connector Server Name value",
    "exchangeConnectorType": "String",
    "version": "Version value",
    "exchangeAlias": "Exchange Alias value",
    "exchangeOrganization": "Exchange Organization value"
  }
}
```

