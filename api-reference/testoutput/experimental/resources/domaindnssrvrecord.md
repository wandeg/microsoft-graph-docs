---
title: "domainDnsSrvRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# domainDnsSrvRecord resource type


Namespace: microsoft.graph




Inherits from [domainDnsRecord](../resources/domaindnsrecord.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainDnsSrvRecords](../api/domaindnssrvrecord-list.md)|[domainDnsSrvRecord](../resources/domaindnssrvrecord.md) collection|List properties and relationships of the [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) objects.|
|[Get domainDnsSrvRecord](../api/domaindnssrvrecord-get.md)|[domainDnsSrvRecord](../resources/domaindnssrvrecord.md)|Read properties and relationships of the [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object.|
|[Create domainDnsSrvRecord](../api/domaindnssrvrecord-create.md)|[domainDnsSrvRecord](../resources/domaindnssrvrecord.md)|Create a new [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object.|
|[Delete domainDnsSrvRecord](../api/domaindnssrvrecord-delete.md)|None|Deletes a [domainDnsSrvRecord](../resources/domaindnssrvrecord.md).|
|[Update domainDnsSrvRecord](../api/domaindnssrvrecord-update.md)|[domainDnsSrvRecord](../resources/domaindnssrvrecord.md)|Update the properties of a [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|nameTarget|String||
|port|Int32||
|priority|Int32||
|protocol|String||
|recordType|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|service|String||
|supportedService|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|ttl|Int32| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|weight|Int32||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.domainDnsSrvRecord",
  "baseType": "microsoft.graph.domainDnsRecord",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainDnsSrvRecord",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024,
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "service": "String",
  "weight": 1024
}
```

