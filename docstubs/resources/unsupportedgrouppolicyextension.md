---
title: "unsupportedGroupPolicyExtension resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# unsupportedGroupPolicyExtension resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get unsupportedGroupPolicyExtension](../api/unsupportedgrouppolicyextension-get.md)|[unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md)|Read properties and relationships of the [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) object.|
|[Update unsupportedGroupPolicyExtension](../api/unsupportedgrouppolicyextension-update.md)|[unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md)|Update the properties of a [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|extensionType|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|namespaceUrl|String||
|nodeName|String||
|settingScope|Enumeration| Possible values are: `unknown`, `device`, `user`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unsupportedGroupPolicyExtension",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "id": "String (identifier)",
  "settingScope": "String",
  "namespaceUrl": "String",
  "extensionType": "String",
  "nodeName": "String"
}
```

