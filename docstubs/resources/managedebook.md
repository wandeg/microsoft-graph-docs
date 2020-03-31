---
title: "managedEBook resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedEBook resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedEBook](../api/managedebook-get.md)|[managedEBook](../resources/managedebook.md)|Read properties and relationships of the [managedEBook](../resources/managedebook.md) object.|
|[assign](../api/managedebook-assign.md)|None||
|[List categories](../api/managedebook-list-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md) collection|Get the managedEBookCategories from the categories navigation property.|
|[Create categories](../api/managedebook-post-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/managedebook-list-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md) collection|Get the managedEBookAssignments from the assignments navigation property.|
|[Add assignments](../api/managedebook-post-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Add assignments by posting to the assignments collection.|
|[Get eBookInstallSummary](../api/ebookinstallsummary-get.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Read properties and relationships of the [eBookInstallSummary](../resources/ebookinstallsummary.md) object.|
|[List deviceStates](../api/managedebook-list-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md) collection|Get the deviceInstallStates from the deviceStates navigation property.|
|[Add deviceStates](../api/managedebook-post-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Add deviceStates by posting to the deviceStates collection.|
|[List userStateSummary](../api/managedebook-list-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection|Get the userInstallStateSummaries from the userStateSummary navigation property.|
|[Add userStateSummary](../api/managedebook-post-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Add userStateSummary by posting to the userStateSummary collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String||
|largeCover|[mimeContent](../resources/mimecontent.md)||
|lastModifiedDateTime|DateTimeOffset||
|privacyInformationUrl|String||
|publishedDateTime|DateTimeOffset||
|publisher|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/managedebookassignment.md) collection||
|categories|[managedEBookCategory](../resources/managedebookcategory.md) collection||
|deviceStates|[deviceInstallState](../resources/deviceinstallstate.md) collection||
|installSummary|[eBookInstallSummary](../resources/ebookinstallsummary.md)||
|userStateSummary|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```

