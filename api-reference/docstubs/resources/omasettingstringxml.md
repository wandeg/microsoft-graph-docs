---
title: "omaSettingStringXml resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# omaSettingStringXml resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [omaSetting](../resources/omasetting.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description. Inherited from [omaSetting](../resources/omasetting.md)|
|displayName|String|Display Name. Inherited from [omaSetting](../resources/omasetting.md)|
|fileName|String|File name associated with the Value property (*.xml).|
|omaUri|String|OMA. Inherited from [omaSetting](../resources/omasetting.md)|
|value|Binary|Value. (UTF8 encoded byte array)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```

