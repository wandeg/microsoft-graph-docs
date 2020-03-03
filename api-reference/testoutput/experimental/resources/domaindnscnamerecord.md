---
title: "domainDnsCnameRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# domainDnsCnameRecord resource type




Inherits from [domainDnsRecord](../resources/domainDnsRecord.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainDnsCnameRecords](../api/domaindnscnamerecord-list.md)|[domainDnsCnameRecord](../resources/domainDnsCnameRecord.md) collection|List properties and relationships of the [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) objects.|
|[Get domainDnsCnameRecord](../api/domaindnscnamerecord-get.md)|[domainDnsCnameRecord](../resources/domainDnsCnameRecord.md)|Read properties and relationships of the [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) object.|
|[Create domainDnsCnameRecord](../api/domaindnscnamerecord-create.md)|[domainDnsCnameRecord](../resources/domainDnsCnameRecord.md)|Create a new [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) object.|
|[Delete domainDnsCnameRecord](../api/domaindnscnamerecord-delete.md)|None|Deletes a [domainDnsCnameRecord](../resources/domaindnscnamerecord.md).|
|[Update domainDnsCnameRecord](../api/domaindnscnamerecord-update.md)|[domainDnsCnameRecord](../resources/domainDnsCnameRecord.md)|Update the properties of a [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|canonicalName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|recordType|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|supportedService|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|ttl|Int32| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|

## Relationships
None

## JSON Representation
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

