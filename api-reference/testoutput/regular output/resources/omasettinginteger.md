---
title: "omaSettingInteger resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# omaSettingInteger resource type




Inherits from [omaSetting](../resources/omaSetting.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description. Inherited from [omaSetting](../resources/omaSetting.md)|
|displayName|String|Display Name. Inherited from [omaSetting](../resources/omaSetting.md)|
|omaUri|String|OMA. Inherited from [omaSetting](../resources/omaSetting.md)|
|value|Int32|Value.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```

