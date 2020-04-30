---
title: "outlookUser resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# outlookUser resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md)|[localeInfo](../resources/localeinfo.md) collection|**TODO: Add Description**|
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md)|[timeZoneInformation](../resources/timezoneinformation.md) collection|**TODO: Add Description**|
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md)|[timeZoneInformation](../resources/timezoneinformation.md) collection|**TODO: Add Description**|
|[List masterCategories](../api/outlookuser-list-mastercategories.md)|[outlookCategory](../resources/outlookcategory.md) collection|Get the outlookCategories from the masterCategories navigation property.|
|[Create masterCategories](../api/outlookuser-post-mastercategories.md)|[outlookCategory](../resources/outlookcategory.md)|Create a new masterCategories object.|
|[Delete masterCategories](../api/outlookuser-delete-mastercategories.md)|None|Delete a [outlookCategory](../resources/outlookcategory.md) object.|
|[Update masterCategories](../api/outlookuser-update-mastercategories.md)|[outlookCategory](../resources/outlookcategory.md)|Update the properties of a masterCategories object.|
|[Get outlookCategory](../api/outlookcategory-get.md)|[outlookCategory](../resources/outlookcategory.md)|Read the properties and relationships of an [outlookCategory](../resources/outlookcategory.md) object.|
|[List taskGroups](../api/outlookuser-list-taskgroups.md)|[outlookTaskGroup](../resources/outlooktaskgroup.md) collection|Get the outlookTaskGroups from the taskGroups navigation property.|
|[Create taskGroups](../api/outlookuser-post-taskgroups.md)|[outlookTaskGroup](../resources/outlooktaskgroup.md)|Create a new taskGroups object.|
|[Delete taskGroups](../api/outlookuser-delete-taskgroups.md)|None|Delete a [outlookTaskGroup](../resources/outlooktaskgroup.md) object.|
|[Update taskGroups](../api/outlookuser-update-taskgroups.md)|[outlookTaskGroup](../resources/outlooktaskgroup.md)|Update the properties of a taskGroups object.|
|[Get outlookTaskGroup](../api/outlooktaskgroup-get.md)|[outlookTaskGroup](../resources/outlooktaskgroup.md)|Read the properties and relationships of an [outlookTaskGroup](../resources/outlooktaskgroup.md) object.|
|[List taskFolders](../api/outlookuser-list-taskfolders.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md) collection|Get the outlookTaskFolders from the taskFolders navigation property.|
|[Create taskFolders](../api/outlookuser-post-taskfolders.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Create a new taskFolders object.|
|[Delete taskFolders](../api/outlookuser-delete-taskfolders.md)|None|Delete a [outlookTaskFolder](../resources/outlooktaskfolder.md) object.|
|[Update taskFolders](../api/outlookuser-update-taskfolders.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Update the properties of a taskFolders object.|
|[Get outlookTaskFolder](../api/outlooktaskfolder-get.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Read the properties and relationships of an [outlookTaskFolder](../resources/outlooktaskfolder.md) object.|
|[List tasks](../api/outlookuser-list-tasks.md)|[outlookTask](../resources/outlooktask.md) collection|Get the outlookTasks from the tasks navigation property.|
|[Create tasks](../api/outlookuser-post-tasks.md)|[outlookTask](../resources/outlooktask.md)|Create a new tasks object.|
|[Delete tasks](../api/outlookuser-delete-tasks.md)|None|Delete a [outlookTask](../resources/outlooktask.md) object.|
|[Update tasks](../api/outlookuser-update-tasks.md)|[outlookTask](../resources/outlooktask.md)|Update the properties of a tasks object.|
|[Get outlookTask](../api/outlooktask-get.md)|[outlookTask](../resources/outlooktask.md)|Read the properties and relationships of an [outlookTask](../resources/outlooktask.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|masterCategories|[outlookCategory](../resources/outlookcategory.md) collection|**TODO: Add Description**|
|taskFolders|[outlookTaskFolder](../resources/outlooktaskfolder.md) collection|**TODO: Add Description**|
|taskGroups|[outlookTaskGroup](../resources/outlooktaskgroup.md) collection|**TODO: Add Description**|
|tasks|[outlookTask](../resources/outlooktask.md) collection|**TODO: Add Description**|

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

