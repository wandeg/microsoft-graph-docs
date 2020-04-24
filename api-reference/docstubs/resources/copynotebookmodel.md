---
title: "CopyNotebookModel resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# CopyNotebookModel resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|String|**TODO: Add Description**|
|createdByIdentity|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|createdTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|
|isShared|Boolean|**TODO: Add Description**|
|lastModifiedBy|String|**TODO: Add Description**|
|lastModifiedByIdentity|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|lastModifiedTime|DateTimeOffset|**TODO: Add Description**|
|links|[notebookLinks](../resources/notebooklinks.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|sectionGroupsUrl|String|**TODO: Add Description**|
|sectionsUrl|String|**TODO: Add Description**|
|self|String|**TODO: Add Description**|
|userRole|onenoteUserRole|**TODO: Add Description**. Possible values are: `Owner`, `Contributor`, `Reader`, `None`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.CopyNotebookModel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.CopyNotebookModel",
  "isDefault": true,
  "userRole": "String",
  "isShared": true,
  "sectionsUrl": "String",
  "sectionGroupsUrl": "String",
  "links": {
    "@odata.type": "microsoft.graph.notebookLinks",
    "oneNoteClientUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "String"
    },
    "oneNoteWebUrl": {
      "@odata.type": "microsoft.graph.externalLink"
    }
  },
  "name": "String",
  "createdBy": "String",
  "createdByIdentity": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedBy": "String",
  "lastModifiedByIdentity": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedTime": "String (timestamp)",
  "id": "String (identifier)",
  "self": "String",
  "createdTime": "String (timestamp)"
}
```

