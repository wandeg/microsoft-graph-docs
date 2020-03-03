---
title: "domainDnsTxtRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# domainDnsTxtRecord resource type


Namespace: microsoft.graph




Inherits from [domainDnsRecord](../resources/domaindnsrecord.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainDnsTxtRecords](../api/domaindnstxtrecord-list.md)|[domainDnsTxtRecord](../resources/domaindnstxtrecord.md) collection|List properties and relationships of the [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) objects.|
|[Get domainDnsTxtRecord](../api/domaindnstxtrecord-get.md)|[domainDnsTxtRecord](../resources/domaindnstxtrecord.md)|Read properties and relationships of the [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) object.|
|[Create domainDnsTxtRecord](../api/domaindnstxtrecord-create.md)|[domainDnsTxtRecord](../resources/domaindnstxtrecord.md)|Create a new [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) object.|
|[Delete domainDnsTxtRecord](../api/domaindnstxtrecord-delete.md)|None|Deletes a [domainDnsTxtRecord](../resources/domaindnstxtrecord.md).|
|[Update domainDnsTxtRecord](../api/domaindnstxtrecord-update.md)|[domainDnsTxtRecord](../resources/domaindnstxtrecord.md)|Update the properties of a [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|recordType|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|supportedService|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|text|String||
|ttl|Int32| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.domainDnsTxtRecord",
  "baseType": "microsoft.graph.domainDnsRecord",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainDnsTxtRecord",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024,
  "text": "String"
}
```

