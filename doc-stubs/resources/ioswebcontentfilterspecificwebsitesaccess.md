---
title: "iosWebContentFilterSpecificWebsitesAccess resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# iosWebContentFilterSpecificWebsitesAccess resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [iosWebContentFilterBase](../resources/ioswebcontentfilterbase.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|specificWebsitesOnly|[iosBookmark](../resources/iosbookmark.md) collection|**TODO: Add Description**|
|websiteList|[iosBookmark](../resources/iosbookmark.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.iosBookmark"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark"
    }
  ]
}
```

