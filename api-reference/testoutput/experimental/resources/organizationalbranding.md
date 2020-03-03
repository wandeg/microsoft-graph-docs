---
title: "organizationalBranding resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# organizationalBranding resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get organizationalBranding](../api/organizationalbranding-get.md)|[organizationalBranding](../resources/organizationalBranding.md)|Read properties and relationships of the [organizationalBranding](../resources/organizationalbranding.md) object.|
|[Delete organizationalBranding](../api/organizationalbranding-delete.md)|None|Deletes a [organizationalBranding](../resources/organizationalbranding.md).|
|[Update organizationalBranding](../api/organizationalbranding-update.md)|[organizationalBranding](../resources/organizationalBranding.md)|Update the properties of a [organizationalBranding](../resources/organizationalbranding.md) object.|
|[List brandings](../api/organization-list-brandings.md)|[organizationalBranding](../resources/organizationalBranding.md) collection|Get the organizationalBrandings from the brandings navigation property.|
|[Add brandings](../api/organization-post-brandings.md)|[organizationalBranding](../resources/organizationalBranding.md)|Add brandings by posting to the brandings collection.|

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

## JSON Representation
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

