---
title: "iosWebContentFilterSpecificWebsitesAccess resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosWebContentFilterSpecificWebsitesAccess resource type


Namespace: microsoft.graph




Inherits from [iosWebContentFilterBase](../resources/ioswebcontentfilterbase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|specificWebsitesOnly|[iosBookmark](../resources/iosbookmark.md) collection||
|websiteList|[iosBookmark](../resources/iosbookmark.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark"
    }
  ]
}
```

