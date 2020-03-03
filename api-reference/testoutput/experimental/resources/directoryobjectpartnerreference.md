---
title: "directoryObjectPartnerReference resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# directoryObjectPartnerReference resource type

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryObject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directoryObjectPartnerReferences](../api/directoryobjectpartnerreference-list.md)|[directoryObjectPartnerReference](../resources/directoryObjectPartnerReference.md) collection|List properties and relationships of the [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) objects.|
|[Get directoryObjectPartnerReference](../api/directoryobjectpartnerreference-get.md)|[directoryObjectPartnerReference](../resources/directoryObjectPartnerReference.md)|Read properties and relationships of the [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object.|
|[Create directoryObjectPartnerReference](../api/directoryobjectpartnerreference-create.md)|[directoryObjectPartnerReference](../resources/directoryObjectPartnerReference.md)|Create a new [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object.|
|[Delete directoryObjectPartnerReference](../api/directoryobjectpartnerreference-delete.md)|None|Deletes a [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md).|
|[Update directoryObjectPartnerReference](../api/directoryobjectpartnerreference-update.md)|[directoryObjectPartnerReference](../resources/directoryObjectPartnerReference.md)|Update the properties of a [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object.|
|[checkMemberGroups](../api/directoryobjectpartnerreference-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/directoryobjectpartnerreference-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/directoryobjectpartnerreference-getmembergroups.md)|String collection||
|[getMemberObjects](../api/directoryobjectpartnerreference-getmemberobjects.md)|String collection||
|[restore](../api/directoryobjectpartnerreference-restore.md)|[directoryObject](../resources/directoryObject.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryObject.md)|
|description|String||
|displayName|String||
|externalPartnerTenantId|Guid||
|id|String| Inherited from [entity](../resources/entity.md)|
|objectType|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference",
  "baseType": "microsoft.graph.directoryObject",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directoryObjectPartnerReference",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "externalPartnerTenantId": "Guid",
  "objectType": "String"
}
```

