---
title: "deviceManagementDomainJoinConnector resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementDomainJoinConnector resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementDomainJoinConnector](../api/devicemanagementdomainjoinconnector-get.md)|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md)|Read properties and relationships of the [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.|
|[Update deviceManagementDomainJoinConnector](../api/devicemanagementdomainjoinconnector-update.md)|[deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md)|Update the properties of a [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset||
|state|Enumeration| Possible values are: `active`, `error`, `inactive`.|
|version|String||

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

