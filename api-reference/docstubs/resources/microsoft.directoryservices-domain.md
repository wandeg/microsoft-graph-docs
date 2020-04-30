---
title: "domain resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# domain resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domains](../api/microsoft.directoryservices-domain-list.md)|[domain](../resources/microsoft.directoryservices-domain.md) collection|Get a list of the [domain](../resources/domain.md) objects and their properties.|
|[Get domain](../api/microsoft.directoryservices-domain-get.md)|[domain](../resources/microsoft.directoryservices-domain.md)|Read properties and relationships of a [domain](../resources/microsoft.directoryservices-domain.md) object.|
|[Create domain](../api/microsoft.directoryservices-domain-post-domains.md)|[domain](../resources/microsoft.directoryservices-domain.md)|Create a new [domain](../resources/microsoft.directoryservices-domain.md) object.|
|[Delete domain](../api/microsoft.directoryservices-domain-delete.md)|None|Deletes a [domain](../resources/microsoft.directoryservices-domain.md).|
|[Update domain](../api/microsoft.directoryservices-domain-update.md)|[domain](../resources/microsoft.directoryservices-domain.md)|Update the properties of a [domain](../resources/microsoft.directoryservices-domain.md) object.|
|[forceDelete](../api/microsoft.directoryservices-domain-forcedelete.md)|None|**TODO: Add Description**|
|[verify](../api/microsoft.directoryservices-domain-verify.md)|[domain](../resources/microsoft.directoryservices-domain.md)|**TODO: Add Description**|
|[List serviceConfigurationRecords](../api/microsoft.directoryservices-domain-list-serviceconfigurationrecords.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) collection|Get the domainDnsRecords from the serviceConfigurationRecords navigation property.|
|[Create serviceConfigurationRecords](../api/microsoft.directoryservices-domain-post-serviceconfigurationrecords.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md)|Create a new serviceConfigurationRecords object.|
|[Delete serviceConfigurationRecords](../api/microsoft.directoryservices-domain-delete-serviceconfigurationrecords.md)|None|Delete a serviceConfigurationRecords object.|
|[Update serviceConfigurationRecords](../api/microsoft.directoryservices-domain-update-serviceconfigurationrecords.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md)|Update the properties of a serviceConfigurationRecords object.|
|[Get domainDnsRecord](../api/microsoft.directoryservices-domaindnsrecord-get.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md)|Read properties and relationships of a [domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) object.|
|[List verificationDnsRecords](../api/microsoft.directoryservices-domain-list-verificationdnsrecords.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) collection|Get the domainDnsRecords from the verificationDnsRecords navigation property.|
|[Create verificationDnsRecords](../api/microsoft.directoryservices-domain-post-verificationdnsrecords.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md)|Create a new verificationDnsRecords object.|
|[Delete verificationDnsRecords](../api/microsoft.directoryservices-domain-delete-verificationdnsrecords.md)|None|Delete a verificationDnsRecords object.|
|[Update verificationDnsRecords](../api/microsoft.directoryservices-domain-update-verificationdnsrecords.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md)|Update the properties of a verificationDnsRecords object.|
|[Get domainDnsRecord](../api/microsoft.directoryservices-domaindnsrecord-get.md)|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md)|Read properties and relationships of a [domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) object.|
|[List domainNameReferences](../api/microsoft.directoryservices-domain-list-domainnamereferences.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the domainNameReferences navigation property.|
|[Add domainNameReferences](../api/microsoft.directoryservices-domain-post-domainnamereferences.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add domainNameReferences by posting to the domainNameReferences collection.|
|[Remove domainNameReferences](../api/microsoft.directoryservices-domain-delete-domainnamereferences.md)|None|Remove a domainNameReferences object.|

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
|passwordNotificationWindowInDays|Int32|**TODO: Add Description**|
|passwordValidityPeriodInDays|Int32|**TODO: Add Description**|
|state|[domainState](../resources/microsoft.directoryservices-domainstate.md)|**TODO: Add Description**|
|supportedServices|String collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|domainNameReferences|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|serviceConfigurationRecords|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) collection|**TODO: Add Description**|
|verificationDnsRecords|[domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.domain",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.domain",
  "authenticationType": "String",
  "availabilityStatus": "String",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "id": "String (identifier)",
  "passwordNotificationWindowInDays": 1024,
  "passwordValidityPeriodInDays": 1024,
  "supportedServices": [
    "String"
  ],
  "state": {
    "@odata.type": "Microsoft.DirectoryServices.domainState",
    "status": "String",
    "operation": "String",
    "lastActionDateTime": "String (timestamp)"
  }
}
```

