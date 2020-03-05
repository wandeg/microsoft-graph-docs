---
title: "deviceManagementExchangeConnector resource type"
description: "Entity which represents a connection to an Exchange environment."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementExchangeConnector resource type


Namespace: microsoft.graph

Entity which represents a connection to an Exchange environment.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementExchangeConnectors](../api/devicemanagementexchangeconnector-list.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) collection|List properties and relationships of the [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) objects.|
|[Get deviceManagementExchangeConnector](../api/devicemanagementexchangeconnector-get.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md)|Read properties and relationships of the [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object.|
|[Create deviceManagementExchangeConnector](../api/devicemanagementexchangeconnector-create.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md)|Create a new [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object.|
|[Delete deviceManagementExchangeConnector](../api/devicemanagementexchangeconnector-delete.md)|None|Deletes a [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md).|
|[Update deviceManagementExchangeConnector](../api/devicemanagementexchangeconnector-update.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md)|Update the properties of a [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object.|
|[sync](../api/devicemanagementexchangeconnector-sync.md)|None||
|[List exchangeConnectors](../api/devicemanagement-list-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) collection|Get the deviceManagementExchangeConnectors from the exchangeConnectors navigation property.|
|[Add exchangeConnectors](../api/devicemanagement-post-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md)|Add exchangeConnectors by posting to the exchangeConnectors collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|connectorServerName|String|The name of the server hosting the Exchange Connector.|
|exchangeAlias|String|An alias assigned to the Exchange server|
|exchangeConnectorType|Enumeration|The type of Exchange Connector Configured. Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|exchangeOrganization|String|Exchange Organization to the Exchange server|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|Last sync time for the Exchange Connector|
|primarySmtpAddress|String|Email address used to configure the Service To Service Exchange Connector.|
|serverName|String|The name of the Exchange server.|
|status|Enumeration|Exchange Connector Status. Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.|
|version|String|The version of the ExchangeConnectorAgent|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeConnector",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "status": "String",
  "primarySmtpAddress": "String",
  "serverName": "String",
  "connectorServerName": "String",
  "exchangeConnectorType": "String",
  "version": "String",
  "exchangeAlias": "String",
  "exchangeOrganization": "String"
}
```

