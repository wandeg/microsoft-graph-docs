---
title: "domainDnsRecord resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# domainDnsRecord resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainDnsRecords](../api/microsoft.directoryservices-domaindnsrecord-list.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) collection|Get a list of the [domainDnsRecord](../resources/domaindnsrecord.md) objects and their properties.|
|[Get domainDnsRecord](../api/microsoft.directoryservices-domaindnsrecord-get.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md)|Read properties and relationships of a [domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) object.|
|[Create domainDnsRecord](../api/microsoft.directoryservices-domaindnsrecord-post-domaindnsrecords.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md)|Create a new [domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) object.|
|[Delete domainDnsRecord](../api/microsoft.directoryservices-domaindnsrecord-delete.md)|None|Deletes a [domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md).|
|[Update domainDnsRecord](../api/microsoft.directoryservices-domaindnsrecord-update.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md)|Update the properties of a [domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|isOptional|Boolean|**TODO: Add Description**|
|label|String|**TODO: Add Description**|
|recordType|String|**TODO: Add Description**|
|supportedService|String|**TODO: Add Description**|
|ttl|Int32|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.domainDnsRecord",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.domainDnsRecord",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}
```

