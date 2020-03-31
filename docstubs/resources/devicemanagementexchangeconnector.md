---
title: "deviceManagementExchangeConnector resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementExchangeConnector resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementExchangeConnector](../api/devicemanagementexchangeconnector-get.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md)|Read properties and relationships of the [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object.|
|[Update deviceManagementExchangeConnector](../api/devicemanagementexchangeconnector-update.md)|[deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md)|Update the properties of a [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object.|
|[sync](../api/devicemanagementexchangeconnector-sync.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|connectorServerName|String||
|exchangeAlias|String||
|exchangeConnectorType|Enumeration| Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|exchangeOrganization|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset||
|primarySmtpAddress|String||
|serverName|String||
|status|Enumeration| Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.|
|version|String||

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

