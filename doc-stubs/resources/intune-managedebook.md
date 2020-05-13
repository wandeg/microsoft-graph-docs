---
title: "managedEBook resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedEBook resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[assign](../api/intune-managedebook-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/intune-managedebook-list-assignments.md)|[managedEBookAssignment](../resources/intune-managedebookassignment.md) collection|Get the managedEBookAssignments from the assignments navigation property.|
|[Create assignments](../api/intune-managedebook-post-assignments.md)|[managedEBookAssignment](../resources/intune-managedebookassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/intune-managedebook-delete-assignments.md)|None|Delete a [managedEBookAssignment](../resources/intune-managedebookassignment.md) object.|
|[Update assignments](../api/intune-managedebook-update-assignments.md)|[managedEBookAssignment](../resources/intune-managedebookassignment.md)|Update the properties of an assignments object.|
|[Get assignments](../api/intune-managedebook-get-managedebookassignment.md)|[managedEBookAssignment](../resources/intune-managedebookassignment.md)|Read the properties and relationships of a [managedEBookAssignment](../resources/intune-managedebookassignment.md) object.|
|[List installSummary](../api/intune-managedebook-list-installsummary.md)|[eBookInstallSummary](../resources/intune-ebookinstallsummary.md) collection|Get the eBookInstallSummaries from the installSummary navigation property.|
|[Create installSummary](../api/intune-managedebook-post-installsummary.md)|[eBookInstallSummary](../resources/intune-ebookinstallsummary.md)|Create a new installSummary object.|
|[Delete installSummary](../api/intune-managedebook-delete-installsummary.md)|None|Delete an [eBookInstallSummary](../resources/intune-ebookinstallsummary.md) object.|
|[Update installSummary](../api/intune-managedebook-update-installsummary.md)|[eBookInstallSummary](../resources/intune-ebookinstallsummary.md)|Update the properties of an installSummary object.|
|[Get installSummary](../api/intune-managedebook-get-ebookinstallsummary.md)|[eBookInstallSummary](../resources/intune-ebookinstallsummary.md)|Read the properties and relationships of an [eBookInstallSummary](../resources/intune-ebookinstallsummary.md) object.|
|[List deviceStates](../api/intune-managedebook-list-devicestates.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md) collection|Get the deviceInstallStates from the deviceStates navigation property.|
|[Create deviceStates](../api/intune-managedebook-post-devicestates.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md)|Create a new deviceStates object.|
|[Delete deviceStates](../api/intune-managedebook-delete-devicestates.md)|None|Delete a [deviceInstallState](../resources/intune-deviceinstallstate.md) object.|
|[Update deviceStates](../api/intune-managedebook-update-devicestates.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md)|Update the properties of a deviceStates object.|
|[Get deviceStates](../api/intune-managedebook-get-deviceinstallstate.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md)|Read the properties and relationships of a [deviceInstallState](../resources/intune-deviceinstallstate.md) object.|
|[List userStateSummary](../api/intune-managedebook-list-userstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md) collection|Get the userInstallStateSummaries from the userStateSummary navigation property.|
|[Create userStateSummary](../api/intune-managedebook-post-userstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md)|Create a new userStateSummary object.|
|[Delete userStateSummary](../api/intune-managedebook-delete-userstatesummary.md)|None|Delete a [userInstallStateSummary](../resources/intune-userinstallstatesummary.md) object.|
|[Update userStateSummary](../api/intune-managedebook-update-userstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md)|Update the properties of a userStateSummary object.|
|[Get userStateSummary](../api/intune-managedebook-get-userinstallstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md)|Read the properties and relationships of a [userInstallStateSummary](../resources/intune-userinstallstatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|informationUrl|String|**TODO: Add Description**|
|largeCover|[mimeContent](../resources/intune-mimecontent.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|privacyInformationUrl|String|**TODO: Add Description**|
|publishedDateTime|DateTimeOffset|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/intune-managedebookassignment.md) collection|**TODO: Add Description**|
|deviceStates|[deviceInstallState](../resources/intune-deviceinstallstate.md) collection|**TODO: Add Description**|
|installSummary|[eBookInstallSummary](../resources/intune-ebookinstallsummary.md)|**TODO: Add Description**|
|userStateSummary|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```

