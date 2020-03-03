---
title: "deviceManagementDomainJoinConnector resource type"
description: "A Domain Join Connector is a connector that is responsible to allocate (and delete) machine account blobs"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementDomainJoinConnector resource type

A Domain Join Connector is a connector that is responsible to allocate (and delete) machine account blobs


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementDomainJoinConnector](../api/devicemanagementdomainjoinconnector-get.md)|[deviceManagementDomainJoinConnector](../resources/deviceManagementDomainJoinConnector.md)|Read properties and relationships of the [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.|
|[Delete deviceManagementDomainJoinConnector](../api/devicemanagementdomainjoinconnector-delete.md)|None|Deletes a [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md).|
|[Update deviceManagementDomainJoinConnector](../api/devicemanagementdomainjoinconnector-update.md)|[deviceManagementDomainJoinConnector](../resources/deviceManagementDomainJoinConnector.md)|Update the properties of a [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.|
|[List domainJoinConnectors](../api/intune-devices-devicemanagement-list-domainjoinconnectors.md)|[deviceManagementDomainJoinConnector](../resources/deviceManagementDomainJoinConnector.md) collection|Get the deviceManagementDomainJoinConnectors from the domainJoinConnectors navigation property.|
|[Add domainJoinConnectors](../api/intune-devices-devicemanagement-post-domainjoinconnectors.md)|[deviceManagementDomainJoinConnector](../resources/deviceManagementDomainJoinConnector.md)|Add domainJoinConnectors by posting to the domainJoinConnectors collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The connector display name.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset|Last time connector contacted Intune.|
|state|Enumeration|The connector state. Possible values are: `active`, `error`, `inactive`.|
|version|String|The version of the connector.|

## Relationships
None

## JSON Representation
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

