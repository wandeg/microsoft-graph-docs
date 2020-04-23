---
title: "Create exchangeConnectors"
description: "Create a new exchangeConnectors object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create exchangeConnectors

Namespace: microsoft.graph

Create a new exchangeConnectors object.

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
POST /deviceManagement/exchangeConnectors
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object.

The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|Last sync time for the Exchange Connector|
|status|deviceManagementExchangeConnectorStatus|Exchange Connector Status. Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.|
|primarySmtpAddress|String|Email address used to configure the Service To Service Exchange Connector.|
|serverName|String|The name of the Exchange server.|
|connectorServerName|String|The name of the server hosting the Exchange Connector.|
|exchangeConnectorType|deviceManagementExchangeConnectorType|The type of Exchange Connector Configured. Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|version|String|The version of the ExchangeConnectorAgent|
|exchangeAlias|String|An alias assigned to the Exchange server|
|exchangeOrganization|String|Exchange Organization to the Exchange server|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementexchangeconnector_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
Content-Type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:03:21.3080262+03:00",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementexchangeconnector"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "737f9b18-9b18-737f-189b-7f73189b7f73",
  "lastSyncDateTime": "2017-01-01T00:03:21.3080262+03:00",
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

