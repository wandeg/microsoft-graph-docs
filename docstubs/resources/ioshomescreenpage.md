---
title: "iosHomeScreenPage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosHomeScreenPage resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|icons|[iosHomeScreenItem](../resources/ioshomescreenitem.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
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
  ]
}
```

