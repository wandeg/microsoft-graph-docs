---
title: "deviceManagementDomainJoinConnector resource type"
description: "A Domain Join Connector is a connector that is responsible to allocate (and delete) machine account blobs"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementDomainJoinConnector resource type


Namespace: microsoft.graph

A Domain Join Connector is a connector that is responsible to allocate (and delete) machine account blobs


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementDomainJoinConnector](../api/devicemanagementdomainjoinconnector-get.md)|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md)|Read the properties and relationships of a [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.|
|[Update deviceManagementDomainJoinConnector](../api/devicemanagementdomainjoinconnector-update.md)|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md)|Update the properties of a [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The connector display name.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset|Last time connector contacted Intune.|
|state|deviceManagementDomainJoinConnectorState|The connector state. Possible values are: `active`, `error`, `inactive`.|
|version|String|The version of the connector.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDomainJoinConnector",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```

