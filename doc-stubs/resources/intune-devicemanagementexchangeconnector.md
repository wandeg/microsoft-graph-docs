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
|[List exchangeConnectors](../api/intune-devicemanagement-list-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/intune-devicemanagementexchangeconnector.md) collection|Get the deviceManagementExchangeConnectors from the exchangeConnectors navigation property.|
|[Create exchangeConnectors](../api/intune-devicemanagement-post-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/intune-devicemanagementexchangeconnector.md)|Create a new exchangeConnectors object.|
|[Delete exchangeConnectors](../api/intune-devicemanagement-delete-exchangeconnectors.md)|None|Delete a [deviceManagementExchangeConnector](../resources/intune-devicemanagementexchangeconnector.md) object.|
|[Update exchangeConnectors](../api/intune-devicemanagement-update-exchangeconnectors.md)|[deviceManagementExchangeConnector](../resources/intune-devicemanagementexchangeconnector.md)|Update the properties of an exchangeConnectors object.|
|[Get exchangeConnectors](../api/intune-devicemanagement-get-devicemanagementexchangeconnector.md)|[deviceManagementExchangeConnector](../resources/intune-devicemanagementexchangeconnector.md)|Read the properties and relationships of a [deviceManagementExchangeConnector](../resources/intune-devicemanagementexchangeconnector.md) object.|
|[sync](../api/intune-devicemanagementexchangeconnector-sync.md)|None|**TODO: Add Description**|

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

