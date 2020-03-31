---
title: "iosHomeScreenFolder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosHomeScreenFolder resource type


Namespace: microsoft.graph




Inherits from [iosHomeScreenItem](../resources/ioshomescreenitem.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String| Inherited from [iosHomeScreenItem](../resources/ioshomescreenitem.md)|
|pages|[iosHomeScreenFolderPage](../resources/ioshomescreenfolderpage.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
  "displayName": "String",
  "pages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
      "apps": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenApp",
          "bundleID": "String"
        }
      ]
    }
  ]
}
```

