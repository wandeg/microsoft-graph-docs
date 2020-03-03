---
title: "ndesConnector resource type"
description: "Entity which represents an OnPrem Ndes connector."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# ndesConnector resource type

Entity which represents an OnPrem Ndes connector.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get ndesConnector](../api/ndesconnector-get.md)|[ndesConnector](../resources/ndesConnector.md)|Read properties and relationships of the [ndesConnector](../resources/ndesconnector.md) object.|
|[Delete ndesConnector](../api/ndesconnector-delete.md)|None|Deletes a [ndesConnector](../resources/ndesconnector.md).|
|[Update ndesConnector](../api/ndesconnector-update.md)|[ndesConnector](../resources/ndesConnector.md)|Update the properties of a [ndesConnector](../resources/ndesconnector.md) object.|
|[List ndesConnectors](../api/intune-devices-devicemanagement-list-ndesconnectors.md)|[ndesConnector](../resources/ndesConnector.md) collection|Get the ndesConnectors from the ndesConnectors navigation property.|
|[Add ndesConnectors](../api/intune-devices-devicemanagement-post-ndesconnectors.md)|[ndesConnector](../resources/ndesConnector.md)|Add ndesConnectors by posting to the ndesConnectors collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The friendly name of the Ndes Connector.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset|Last connection time for the Ndes Connector|
|state|Enumeration|Ndes Connector Status. Possible values are: `none`, `active`, `inactive`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ndesConnector",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "String (identifier)",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "displayName": "String"
}
```

