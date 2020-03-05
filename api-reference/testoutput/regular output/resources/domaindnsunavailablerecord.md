---
title: "domainDnsUnavailableRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# domainDnsUnavailableRecord resource type


Namespace: microsoft.graph




Inherits from [domainDnsRecord](../resources/domaindnsrecord.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainDnsUnavailableRecords](../api/domaindnsunavailablerecord-list.md)|[domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) collection|List properties and relationships of the [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) objects.|
|[Get domainDnsUnavailableRecord](../api/domaindnsunavailablerecord-get.md)|[domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md)|Read properties and relationships of the [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object.|
|[Create domainDnsUnavailableRecord](../api/domaindnsunavailablerecord-create.md)|[domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md)|Create a new [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object.|
|[Delete domainDnsUnavailableRecord](../api/domaindnsunavailablerecord-delete.md)|None|Deletes a [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md).|
|[Update domainDnsUnavailableRecord](../api/domaindnsunavailablerecord-update.md)|[domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md)|Update the properties of a [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
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

