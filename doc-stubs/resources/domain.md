---
title: "domain resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# domain resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[forceDelete](../api/domain-forcedelete.md)|None|**TODO: Add Description**|
|[verify](../api/domain-verify.md)|[domain](../resources/domain.md)|**TODO: Add Description**|
|[List domainNameReferences](../api/domain-list-domainnamereferences.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the domainNameReferences navigation property.|
|[Add domainNameReferences](../api/domain-post-domainnamereferences.md)|[directoryObject](../resources/directoryobject.md)|Add domainNameReferences by posting to the domainNameReferences collection.|
|[Remove domainNameReferences](../api/domain-delete-domainnamereferences.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md) collection|Get the domainDnsRecords from the serviceConfigurationRecords navigation property.|
|[Create serviceConfigurationRecords](../api/domain-post-serviceconfigurationrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Create a new serviceConfigurationRecords object.|
|[Get serviceConfigurationRecords](../api/domain-get-domaindnsrecord.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Read the properties and relationships of a [domainDnsRecord](../resources/domaindnsrecord.md) object.|
|[Update serviceConfigurationRecords](../api/domain-update-serviceconfigurationrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Update the properties of a serviceConfigurationRecords object.|
|[Delete serviceConfigurationRecords](../api/domain-delete-serviceconfigurationrecords.md)|None|Delete a [domainDnsRecord](../resources/domaindnsrecord.md) object.|
|[List verificationDnsRecords](../api/domain-list-verificationdnsrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md) collection|Get the domainDnsRecords from the verificationDnsRecords navigation property.|
|[Create verificationDnsRecords](../api/domain-post-verificationdnsrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Create a new verificationDnsRecords object.|
|[Get verificationDnsRecords](../api/domain-get-domaindnsrecord.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Read the properties and relationships of a [domainDnsRecord](../resources/domaindnsrecord.md) object.|
|[Update verificationDnsRecords](../api/domain-update-verificationdnsrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Update the properties of a verificationDnsRecords object.|
|[Delete verificationDnsRecords](../api/domain-delete-verificationdnsrecords.md)|None|Delete a [domainDnsRecord](../resources/domaindnsrecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authenticationType|String|**TODO: Add Description**|
|availabilityStatus|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isAdminManaged|Boolean|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|
|isInitial|Boolean|**TODO: Add Description**|
|isRoot|Boolean|**TODO: Add Description**|
|isVerified|Boolean|**TODO: Add Description**|
|manufacturer|String|**TODO: Add Description**|
|model|String|**TODO: Add Description**|
|passwordNotificationWindowInDays|Int32|**TODO: Add Description**|
|passwordValidityPeriodInDays|Int32|**TODO: Add Description**|
|state|[domainState](../resources/domainstate.md)|**TODO: Add Description**|
|supportedServices|String collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|domainNameReferences|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|serviceConfigurationRecords|[domainDnsRecord](../resources/domaindnsrecord.md) collection|**TODO: Add Description**|
|verificationDnsRecords|[domainDnsRecord](../resources/domaindnsrecord.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.domain",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domain",
  "authenticationType": "String",
  "availabilityStatus": "String",
  "isAdminManaged": "Boolean",
  "isDefault": "Boolean",
  "isInitial": "Boolean",
  "isRoot": "Boolean",
  "isVerified": "Boolean",
  "id": "String (identifier)",
  "manufacturer": "String",
  "model": "String",
  "passwordNotificationWindowInDays": "Integer",
  "passwordValidityPeriodInDays": "Integer",
  "supportedServices": [
    "String"
  ],
  "state": {
    "@odata.type": "microsoft.graph.domainState"
  }
}
```

