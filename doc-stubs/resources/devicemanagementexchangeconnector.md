---
title: "deviceManagementExchangeConnector resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementExchangeConnector resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[sync](../api/devicemanagementexchangeconnector-sync.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|connectorServerName|String|**TODO: Add Description**|
|exchangeAlias|String|**TODO: Add Description**|
|exchangeConnectorType|deviceManagementExchangeConnectorType|**TODO: Add Description**. Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|exchangeOrganization|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|primarySmtpAddress|String|**TODO: Add Description**|
|serverName|String|**TODO: Add Description**|
|status|deviceManagementExchangeConnectorStatus|**TODO: Add Description**. Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.|
|version|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

