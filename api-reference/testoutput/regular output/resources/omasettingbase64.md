---
title: "omaSettingBase64 resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# omaSettingBase64 resource type




Inherits from [omaSetting](../resources/omaSetting.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description. Inherited from [omaSetting](../resources/omaSetting.md)|
|displayName|String|Display Name. Inherited from [omaSetting](../resources/omaSetting.md)|
|fileName|String|File name associated with the Value property (*.cer | *.crt | *.p7b | *.bin).|
|omaUri|String|OMA. Inherited from [omaSetting](../resources/omaSetting.md)|
|value|String|Value. (Base64 encoded string)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```

