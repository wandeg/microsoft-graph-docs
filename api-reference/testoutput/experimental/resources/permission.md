---
title: "permission resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# permission resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List permissions](../api/permission-list.md)|[permission](../resources/permission.md) collection|List properties and relationships of the [permission](../resources/permission.md) objects.|
|[Get permission](../api/permission-get.md)|[permission](../resources/permission.md)|Read properties and relationships of the [permission](../resources/permission.md) object.|
|[Create permission](../api/permission-create.md)|[permission](../resources/permission.md)|Create a new [permission](../resources/permission.md) object.|
|[Delete permission](../api/permission-delete.md)|None|Deletes a [permission](../resources/permission.md).|
|[Update permission](../api/permission-update.md)|[permission](../resources/permission.md)|Update the properties of a [permission](../resources/permission.md) object.|
|[grant](../api/permission-grant.md)|[permission](../resources/permission.md) collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset||
|grantedTo|[identitySet](../resources/identityset.md)||
|grantedToIdentities|[identitySet](../resources/identityset.md) collection||
|hasPassword|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|inheritedFrom|[itemReference](../resources/itemreference.md)||
|invitation|[sharingInvitation](../resources/sharinginvitation.md)||
|link|[sharingLink](../resources/sharinglink.md)||
|roles|String collection||
|shareId|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permission",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.permission",
  "id": "String (identifier)",
  "expirationDateTime": "String (timestamp)",
  "grantedTo": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "grantedToIdentities": [
    {
      "@odata.type": "microsoft.graph.identitySet"
    }
  ],
  "hasPassword": true,
  "inheritedFrom": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "invitation": {
    "@odata.type": "microsoft.graph.sharingInvitation"
  },
  "link": {
    "@odata.type": "microsoft.graph.sharingLink"
  },
  "roles": [
    "String"
  ],
  "shareId": "String"
}
```

