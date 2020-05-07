---
title: "protectGroup resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# protectGroup resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [labelActionBase](../resources/labelactionbase.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowEmailFromGuestUsers|Boolean|**TODO: Add Description**|
|allowGuestUsers|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description** Inherited from [labelActionBase](../resources/labelactionbase.md)|
|privacy|groupPrivacy|**TODO: Add Description**. Possible values are: `unspecified`, `public`, `private`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.protectGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.protectGroup",
  "name": "String",
  "allowEmailFromGuestUsers": "Boolean",
  "allowGuestUsers": "Boolean",
  "privacy": "String"
}
```

