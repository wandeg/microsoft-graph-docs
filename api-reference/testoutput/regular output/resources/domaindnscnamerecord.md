---
title: "domainDnsCnameRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# domainDnsCnameRecord resource type


Namespace: microsoft.graph




Inherits from [domainDnsRecord](../resources/domaindnsrecord.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainDnsCnameRecords](../api/domaindnscnamerecord-list.md)|[domainDnsCnameRecord](../resources/domaindnscnamerecord.md) collection|List properties and relationships of the [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) objects.|
|[Get domainDnsCnameRecord](../api/domaindnscnamerecord-get.md)|[domainDnsCnameRecord](../resources/domaindnscnamerecord.md)|Read properties and relationships of the [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) object.|
|[Create domainDnsCnameRecord](../api/domaindnscnamerecord-create.md)|[domainDnsCnameRecord](../resources/domaindnscnamerecord.md)|Create a new [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) object.|
|[Delete domainDnsCnameRecord](../api/domaindnscnamerecord-delete.md)|None|Deletes a [domainDnsCnameRecord](../resources/domaindnscnamerecord.md).|
|[Update domainDnsCnameRecord](../api/domaindnscnamerecord-update.md)|[domainDnsCnameRecord](../resources/domaindnscnamerecord.md)|Update the properties of a [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|canonicalName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|recordType|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|supportedService|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|ttl|Int32| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.domainDnsCnameRecord",
  "baseType": "microsoft.graph.domainDnsRecord",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainDnsCnameRecord",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024,
  "canonicalName": "String"
}
```

