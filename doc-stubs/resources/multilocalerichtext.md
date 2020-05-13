---
title: "MultiLocaleRichText resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# MultiLocaleRichText resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|localized|[RichTextMapElement](../resources/richtextmapelement.md) collection|**TODO: Add Description**|
|preferredLocale|[Locale](../resources/locale.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.MultiLocaleRichText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.MultiLocaleRichText",
  "localized": [
    {
      "@odata.type": "microsoft.graph.RichTextMapElement"
    }
  ],
  "preferredLocale": {
    "@odata.type": "microsoft.graph.Locale"
  }
}
```

