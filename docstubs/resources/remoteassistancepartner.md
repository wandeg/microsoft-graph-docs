---
title: "remoteAssistancePartner resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# remoteAssistancePartner resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get remoteAssistancePartner](../api/remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/remoteassistancepartner.md)|Read properties and relationships of the [remoteAssistancePartner](../resources/remoteassistancepartner.md) object.|
|[Update remoteAssistancePartner](../api/remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/remoteassistancepartner.md)|Update the properties of a [remoteAssistancePartner](../resources/remoteassistancepartner.md) object.|
|[beginOnboarding](../api/remoteassistancepartner-beginonboarding.md)|None||
|[disconnect](../api/remoteassistancepartner-disconnect.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset||
|onboardingStatus|Enumeration| Possible values are: `notOnboarded`, `onboarding`, `onboarded`.|
|onboardingUrl|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```

