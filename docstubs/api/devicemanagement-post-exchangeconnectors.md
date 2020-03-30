---
title: "Add exchangeConnectors"
description: "Add exchangeConnectors by posting to the exchangeConnectors collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add exchangeConnectors

Namespace: microsoft.graph

Add exchangeConnectors by posting to the exchangeConnectors collection.

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
POST /deviceManagement/exchangeConnectors/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object.

The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset||
|status|Enumeration| Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.|
|primarySmtpAddress|String||
|serverName|String||
|connectorServerName|String||
|exchangeConnectorType|Enumeration| Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|version|String||
|exchangeAlias|String||
|exchangeOrganization|String||



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementexchangeconnector_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:01:32.4757974+03:00",
  "status": "String",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "String",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementexchangeconnector"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 528

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "6488f9d4-f9d4-6488-d4f9-8864d4f98864",
  "lastSyncDateTime": "2017-01-01T00:01:32.4757974+03:00",
  "status": "String",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "String",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

