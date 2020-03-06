---
title: "ndesConnector resource type"
description: "Entity which represents an OnPrem Ndes connector."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# ndesConnector resource type


Namespace: microsoft.graph

Entity which represents an OnPrem Ndes connector.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get ndesConnector](../api/ndesconnector-get.md)|[ndesConnector](../resources/ndesconnector.md)|Read properties and relationships of the [ndesConnector](../resources/ndesconnector.md) object.|
|[Update ndesConnector](../api/ndesconnector-update.md)|[ndesConnector](../resources/ndesconnector.md)|Update the properties of a [ndesConnector](../resources/ndesconnector.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The friendly name of the Ndes Connector.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset|Last connection time for the Ndes Connector|
|state|Enumeration|Ndes Connector Status. Possible values are: `none`, `active`, `inactive`.|

## Relationships
None

## JSON representation
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

