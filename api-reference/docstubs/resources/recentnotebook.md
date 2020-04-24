---
title: "recentNotebook resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# recentNotebook resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|lastAccessedTime|DateTimeOffset|**TODO: Add Description**|
|links|[recentNotebookLinks](../resources/recentnotebooklinks.md)|**TODO: Add Description**|
|sourceService|onenoteSourceService|**TODO: Add Description**. Possible values are: `Unknown`, `OneDrive`, `OneDriveForBusiness`, `OnPremOneDriveForBusiness`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.recentNotebook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recentNotebook",
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {
    "@odata.type": "microsoft.graph.recentNotebookLinks",
    "oneNoteClientUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "String"
    },
    "oneNoteWebUrl": {
      "@odata.type": "microsoft.graph.externalLink"
    }
  },
  "sourceService": "String"
}
```

