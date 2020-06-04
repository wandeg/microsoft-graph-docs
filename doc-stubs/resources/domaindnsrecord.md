---
title: "domainDnsRecord resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# domainDnsRecord resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md) collection|Get the domainDnsRecords from the serviceConfigurationRecords navigation property.|
|[Create serviceConfigurationRecords](../api/domain-post-serviceconfigurationrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Create a new serviceConfigurationRecords object.|
|[Update serviceConfigurationRecords](../api/domain-update-serviceconfigurationrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Update the properties of a serviceConfigurationRecords object.|
|[Get serviceConfigurationRecords](../api/domain-get-domaindnsrecord.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Read the properties and relationships of a [domainDnsRecord](../resources/domaindnsrecord.md) object.|
|[Delete serviceConfigurationRecords](../api/domain-delete-serviceconfigurationrecords.md)|None|Delete a [domainDnsRecord](../resources/domaindnsrecord.md) object.|
|[List domainDnsRecords](../api/domaindnsrecord-list.md)|[domainDnsRecord](../resources/domaindnsrecord.md) collection|Get a list of the [domainDnsRecord](../resources/domaindnsrecord.md) objects and their properties.|
|[Create domainDnsRecord](../api/domaindnsrecord-post-domaindnsrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Create a new [domainDnsRecord](../resources/domaindnsrecord.md) object.|
|[Get domainDnsRecord](../api/domaindnsrecord-get.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Read the properties and relationships of a [domainDnsRecord](../resources/domaindnsrecord.md) object.|
|[Update domainDnsRecord](../api/domaindnsrecord-update.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Update the properties of a [domainDnsRecord](../resources/domaindnsrecord.md) object.|
|[Delete domainDnsRecord](../api/domaindnsrecord-delete.md)|None|Deletes a [domainDnsRecord](../resources/domaindnsrecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean|**TODO: Add Description**|
|label|String|**TODO: Add Description**|
|recordType|String|**TODO: Add Description**|
|supportedService|String|**TODO: Add Description**|
|ttl|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "isOptional": "Boolean",
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": "Integer"
}
```

