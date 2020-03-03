---
title: "domainDnsRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# domainDnsRecord resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get domainDnsRecord](../api/domaindnsrecord-get.md)|[domainDnsRecord](../resources/domainDnsRecord.md)|Read properties and relationships of the [domainDnsRecord](../resources/domaindnsrecord.md) object.|
|[Delete domainDnsRecord](../api/domaindnsrecord-delete.md)|None|Deletes a [domainDnsRecord](../resources/domaindnsrecord.md).|
|[Update domainDnsRecord](../api/domaindnsrecord-update.md)|[domainDnsRecord](../resources/domainDnsRecord.md)|Update the properties of a [domainDnsRecord](../resources/domaindnsrecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean||
|label|String||
|recordType|String||
|supportedService|String||
|ttl|Int32||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainDnsRecord",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}
```

