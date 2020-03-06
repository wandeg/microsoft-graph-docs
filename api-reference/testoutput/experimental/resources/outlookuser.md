---
title: "outlookUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# outlookUser resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get outlookUser](../api/outlookuser-get.md)|[outlookUser](../resources/outlookuser.md)|Read properties and relationships of the [outlookUser](../resources/outlookuser.md) object.|
|[Update outlookUser](../api/outlookuser-update.md)|[outlookUser](../resources/outlookuser.md)|Update the properties of a [outlookUser](../resources/outlookuser.md) object.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md)|[localeInfo](../resources/localeinfo.md) collection||
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md)|[timeZoneInformation](../resources/timezoneinformation.md) collection||
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md)|[timeZoneInformation](../resources/timezoneinformation.md) collection||
|[List masterCategories](../api/outlookuser-list-mastercategories.md)|[outlookCategory](../resources/outlookcategory.md) collection|Get the outlookCategories from the masterCategories navigation property.|
|[Add masterCategories](../api/outlookuser-post-mastercategories.md)|[outlookCategory](../resources/outlookcategory.md)|Add masterCategories by posting to the masterCategories collection.|
|[List taskGroups](../api/outlookuser-list-taskgroups.md)|[outlookTaskGroup](../resources/outlooktaskgroup.md) collection|Get the outlookTaskGroups from the taskGroups navigation property.|
|[Add taskGroups](../api/outlookuser-post-taskgroups.md)|[outlookTaskGroup](../resources/outlooktaskgroup.md)|Add taskGroups by posting to the taskGroups collection.|
|[List taskFolders](../api/outlookuser-list-taskfolders.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md) collection|Get the outlookTaskFolders from the taskFolders navigation property.|
|[Add taskFolders](../api/outlookuser-post-taskfolders.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Add taskFolders by posting to the taskFolders collection.|
|[List tasks](../api/outlookuser-list-tasks.md)|[outlookTask](../resources/outlooktask.md) collection|Get the outlookTasks from the tasks navigation property.|
|[Add tasks](../api/outlookuser-post-tasks.md)|[outlookTask](../resources/outlooktask.md)|Add tasks by posting to the tasks collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|masterCategories|[outlookCategory](../resources/outlookcategory.md) collection||
|taskFolders|[outlookTaskFolder](../resources/outlooktaskfolder.md) collection||
|taskGroups|[outlookTaskGroup](../resources/outlooktaskgroup.md) collection||
|tasks|[outlookTask](../resources/outlooktask.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.outlookUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outlookUser",
  "id": "String (identifier)"
}
```

