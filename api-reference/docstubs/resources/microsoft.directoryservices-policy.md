---
title: "policy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# policy resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get policy](../api/microsoft.directoryservices-policy-get.md)|[policy](../resources/microsoft.directoryservices-policy.md)|Read properties and relationships of a [policy](../resources/microsoft.directoryservices-policy.md) object.|
|[Update policy](../api/microsoft.directoryservices-policy-update.md)|[policy](../resources/microsoft.directoryservices-policy.md)|Update the properties of a [policy](../resources/microsoft.directoryservices-policy.md) object.|
|[checkMemberGroups](../api/microsoft.directoryservices-policy-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-policy-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-policy-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-policy-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-policy-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|[List appliesTo](../api/microsoft.directoryservices-policy-list-appliesto.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Add appliesTo](../api/microsoft.directoryservices-policy-post-appliesto.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add appliesTo by posting to the appliesTo collection.|
|[Remove appliesTo](../api/microsoft.directoryservices-policy-delete-appliesto.md)|None|Remove an appliesTo object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alternativeIdentifier|String|**TODO: Add Description**|
|definition|String collection|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description**|
|keyCredentials|[keyCredential](../resources/microsoft.directoryservices-keycredential.md) collection|**TODO: Add Description**|
|type|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.policy",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.policy",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "alternativeIdentifier": "String",
  "definition": [
    "String"
  ],
  "displayName": "String",
  "isOrganizationDefault": true,
  "keyCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.keyCredential",
      "customKeyIdentifier": "binary",
      "endDateTime": "String (timestamp)",
      "keyId": "Guid",
      "startDateTime": "String (timestamp)",
      "usage": "String",
      "key": "binary"
    }
  ],
  "type": "String"
}
```

