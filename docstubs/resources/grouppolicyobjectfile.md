---
title: "groupPolicyObjectFile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyObjectFile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyObjectFile](../api/grouppolicyobjectfile-get.md)|[groupPolicyObjectFile](../resources/grouppolicyobjectfile.md)|Read properties and relationships of the [groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) object.|
|[Update groupPolicyObjectFile](../api/grouppolicyobjectfile-update.md)|[groupPolicyObjectFile](../resources/grouppolicyobjectfile.md)|Update the properties of a [groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyObjectFile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "String (identifier)",
  "content": "String"
}
```

