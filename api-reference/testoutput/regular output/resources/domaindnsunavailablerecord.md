---
title: "domainDnsUnavailableRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# domainDnsUnavailableRecord resource type




Inherits from [domainDnsRecord](../resources/domainDnsRecord.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainDnsUnavailableRecords](../api/domaindnsunavailablerecord-list.md)|[domainDnsUnavailableRecord](../resources/domainDnsUnavailableRecord.md) collection|List properties and relationships of the [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) objects.|
|[Get domainDnsUnavailableRecord](../api/domaindnsunavailablerecord-get.md)|[domainDnsUnavailableRecord](../resources/domainDnsUnavailableRecord.md)|Read properties and relationships of the [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object.|
|[Create domainDnsUnavailableRecord](../api/domaindnsunavailablerecord-create.md)|[domainDnsUnavailableRecord](../resources/domainDnsUnavailableRecord.md)|Create a new [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object.|
|[Delete domainDnsUnavailableRecord](../api/domaindnsunavailablerecord-delete.md)|None|Deletes a [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md).|
|[Update domainDnsUnavailableRecord](../api/domaindnsunavailablerecord-update.md)|[domainDnsUnavailableRecord](../resources/domainDnsUnavailableRecord.md)|Update the properties of a [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
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
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord",
  "baseType": "microsoft.graph.domainDnsRecord",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainDnsUnavailableRecord",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024,
  "description": "String"
}
```

