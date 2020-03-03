---
title: "domainDnsMxRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# domainDnsMxRecord resource type




Inherits from [domainDnsRecord](../resources/domainDnsRecord.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainDnsMxRecords](../api/domaindnsmxrecord-list.md)|[domainDnsMxRecord](../resources/domainDnsMxRecord.md) collection|List properties and relationships of the [domainDnsMxRecord](../resources/domaindnsmxrecord.md) objects.|
|[Get domainDnsMxRecord](../api/domaindnsmxrecord-get.md)|[domainDnsMxRecord](../resources/domainDnsMxRecord.md)|Read properties and relationships of the [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object.|
|[Create domainDnsMxRecord](../api/domaindnsmxrecord-create.md)|[domainDnsMxRecord](../resources/domainDnsMxRecord.md)|Create a new [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object.|
|[Delete domainDnsMxRecord](../api/domaindnsmxrecord-delete.md)|None|Deletes a [domainDnsMxRecord](../resources/domaindnsmxrecord.md).|
|[Update domainDnsMxRecord](../api/domaindnsmxrecord-update.md)|[domainDnsMxRecord](../resources/domainDnsMxRecord.md)|Update the properties of a [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|mailExchange|String||
|preference|Int32||
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
  "@odata.type": "microsoft.graph.domainDnsMxRecord",
  "baseType": "microsoft.graph.domainDnsRecord",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainDnsMxRecord",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024,
  "mailExchange": "String",
  "preference": 1024
}
```

