---
title: "managedEBook resource type"
description: "An abstract class containing the base properties for Managed eBook."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedEBook resource type


Namespace: microsoft.graph

An abstract class containing the base properties for Managed eBook.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedEBook](../api/managedebook-get.md)|[managedEBook](../resources/managedebook.md)|Read the properties and relationships of a [managedEBook](../resources/managedebook.md) object.|
|[assign](../api/managedebook-assign.md)|None|**TODO: Add Description**|
|[List categories](../api/managedebook-list-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md) collection|Get the managedEBookCategories from the categories navigation property.|
|[Add categories](../api/managedebook-post-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Add categories by posting to the categories collection.|
|[Remove categories](../api/managedebook-delete-categories.md)|None|Remove a [managedEBookCategory](../resources/managedebookcategory.md) object.|
|[List assignments](../api/managedebook-list-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md) collection|Get the managedEBookAssignments from the assignments navigation property.|
|[Create assignments](../api/managedebook-post-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/managedebook-delete-assignments.md)|None|Delete an [managedEBookAssignment](../resources/managedebookassignment.md) object.|
|[Update assignments](../api/managedebook-update-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Update the properties of an assignments object.|
|[Get managedEBookAssignment](../api/managedebookassignment-get.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Read the properties and relationships of a [managedEBookAssignment](../resources/managedebookassignment.md) object.|
|[List installSummary](../api/managedebook-list-installsummary.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md) collection|Get the eBookInstallSummaries from the installSummary navigation property.|
|[Create installSummary](../api/managedebook-post-installsummary.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Create a new installSummary object.|
|[Delete installSummary](../api/managedebook-delete-installsummary.md)|None|Delete an [eBookInstallSummary](../resources/ebookinstallsummary.md) object.|
|[Update installSummary](../api/managedebook-update-installsummary.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Update the properties of an installSummary object.|
|[Get eBookInstallSummary](../api/ebookinstallsummary-get.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Read the properties and relationships of an [eBookInstallSummary](../resources/ebookinstallsummary.md) object.|
|[List deviceStates](../api/managedebook-list-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md) collection|Get the deviceInstallStates from the deviceStates navigation property.|
|[Create deviceStates](../api/managedebook-post-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Create a new deviceStates object.|
|[Delete deviceStates](../api/managedebook-delete-devicestates.md)|None|Delete a [deviceInstallState](../resources/deviceinstallstate.md) object.|
|[Update deviceStates](../api/managedebook-update-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Update the properties of a deviceStates object.|
|[Get deviceInstallState](../api/deviceinstallstate-get.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Read the properties and relationships of a [deviceInstallState](../resources/deviceinstallstate.md) object.|
|[List userStateSummary](../api/managedebook-list-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection|Get the userInstallStateSummaries from the userStateSummary navigation property.|
|[Create userStateSummary](../api/managedebook-post-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Create a new userStateSummary object.|
|[Delete userStateSummary](../api/managedebook-delete-userstatesummary.md)|None|Delete a [userInstallStateSummary](../resources/userinstallstatesummary.md) object.|
|[Update userStateSummary](../api/managedebook-update-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Update the properties of a userStateSummary object.|
|[Get userInstallStateSummary](../api/userinstallstatesummary-get.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Read the properties and relationships of a [userInstallStateSummary](../resources/userinstallstatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time when the eBook file was created.|
|description|String|Description.|
|displayName|String|Name of the eBook.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url.|
|largeCover|[mimeContent](../resources/mimecontent.md)|Book cover.|
|lastModifiedDateTime|DateTimeOffset|The date and time when the eBook was last modified.|
|privacyInformationUrl|String|The privacy statement Url.|
|publishedDateTime|DateTimeOffset|The date and time when the eBook was published.|
|publisher|String|Publisher.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/managedebookassignment.md) collection|The list of assignments for this eBook.|
|categories|[managedEBookCategory](../resources/managedebookcategory.md) collection|The list of categories for this eBook.|
|deviceStates|[deviceInstallState](../resources/deviceinstallstate.md) collection|The list of installation states for this eBook.|
|installSummary|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Mobile App Install Summary.|
|userStateSummary|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection|The list of installation states for this eBook.|

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

