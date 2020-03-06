---
title: "organizationalBranding resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# organizationalBranding resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get organizationalBranding](../api/organizationalbranding-get.md)|[organizationalBranding](../resources/organizationalbranding.md)|Read properties and relationships of the [organizationalBranding](../resources/organizationalbranding.md) object.|
|[Update organizationalBranding](../api/organizationalbranding-update.md)|[organizationalBranding](../resources/organizationalbranding.md)|Update the properties of a [organizationalBranding](../resources/organizationalbranding.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|backgroundColor|String||
|backgroundImage|Stream||
|bannerLogo|Stream||
|id|String| Inherited from [entity](../resources/entity.md)|
|locale|String||
|signInPageText|String||
|squareLogo|Stream||
|usernameHintText|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organizationalBranding",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizationalBranding",
  "id": "String (identifier)",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "locale": "String",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
}
```

