---
title: "windowsInformationProtectionNetworkLearningSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionNetworkLearningSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsInformationProtectionNetworkLearningSummary](../api/windowsinformationprotectionnetworklearningsummary-get.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md)|Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) object.|
|[Update windowsInformationProtectionNetworkLearningSummary](../api/windowsinformationprotectionnetworklearningsummary-update.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md)|Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|url|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "String (identifier)",
  "url": "String",
  "deviceCount": 1024
}
```

