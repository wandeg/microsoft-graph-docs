---
title: "domainDnsTxtRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# domainDnsTxtRecord resource type




Inherits from [domainDnsRecord](../resources/domainDnsRecord.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainDnsTxtRecords](../api/domaindnstxtrecord-list.md)|[domainDnsTxtRecord](../resources/domainDnsTxtRecord.md) collection|List properties and relationships of the [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) objects.|
|[Get domainDnsTxtRecord](../api/domaindnstxtrecord-get.md)|[domainDnsTxtRecord](../resources/domainDnsTxtRecord.md)|Read properties and relationships of the [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) object.|
|[Create domainDnsTxtRecord](../api/domaindnstxtrecord-create.md)|[domainDnsTxtRecord](../resources/domainDnsTxtRecord.md)|Create a new [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) object.|
|[Delete domainDnsTxtRecord](../api/domaindnstxtrecord-delete.md)|None|Deletes a [domainDnsTxtRecord](../resources/domaindnstxtrecord.md).|
|[Update domainDnsTxtRecord](../api/domaindnstxtrecord-update.md)|[domainDnsTxtRecord](../resources/domainDnsTxtRecord.md)|Update the properties of a [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|recordType|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|supportedService|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|text|String||
|ttl|Int32| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|

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

