---
title: "printUserIdentity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printUserIdentity resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printUserIdentity](../api/printuseridentity-get.md)|[printUserIdentity](../resources/printuseridentity.md)|Read properties and relationships of the [printUserIdentity](../resources/printuseridentity.md) object.|
|[Update printUserIdentity](../api/printuseridentity-update.md)|[printUserIdentity](../resources/printuseridentity.md)|Update the properties of a [printUserIdentity](../resources/printuseridentity.md) object.|
|[List allowedUsers](../api/printer-list-allowedusers.md)|[printUserIdentity](../resources/printuseridentity.md) collection|Get the printUserIdentities from the allowedUsers navigation property.|
|[Create allowedUsers](../api/printer-post-allowedusers.md)|[printUserIdentity](../resources/printuseridentity.md)|Create allowedUsers by posting to the allowedUsers collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|ipAddress|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUserIdentity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUserIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "ipAddress": "String",
  "userPrincipalName": "String"
}
```

