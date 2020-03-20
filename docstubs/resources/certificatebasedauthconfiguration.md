---
title: "certificateBasedAuthConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# certificateBasedAuthConfiguration resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List certificateBasedAuthConfigurations](../api/certificatebasedauthconfiguration-list.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) collection|List properties and relationships of the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects.|
|[Get certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-get.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)|Read properties and relationships of the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.|
|[Create certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)|Create a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.|
|[Delete certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-delete.md)|None|Deletes a [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md).|
|[Update certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-update.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)|Update the properties of a [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.|
|[List certificateBasedAuthConfiguration](../api/organization-list-certificatebasedauthconfiguration.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) collection|Get the certificateBasedAuthConfigurations from the certificateBasedAuthConfiguration navigation property.|
|[Create certificateBasedAuthConfiguration](../api/organization-post-certificatebasedauthconfiguration.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)|Create certificateBasedAuthConfiguration by posting to the certificateBasedAuthConfiguration collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateAuthorities|[certificateAuthority](../resources/certificateauthority.md) collection||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateBasedAuthConfiguration",
  "id": "String (identifier)",
  "certificateAuthorities": [
    {
      "@odata.type": "microsoft.graph.certificateAuthority"
    }
  ]
}
```

