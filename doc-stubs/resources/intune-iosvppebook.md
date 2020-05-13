---
title: "iosVppEBook resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# iosVppEBook resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [managedEBook](../resources/managedebook.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[assign](../api/intune-iosvppebook-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/intune-iosvppebook-list-assignments.md)|[managedEBookAssignment](../resources/intune-managedebookassignment.md) collection|Get the managedEBookAssignments from the assignments navigation property.|
|[Create assignments](../api/intune-iosvppebook-post-assignments.md)|[managedEBookAssignment](../resources/intune-managedebookassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/intune-iosvppebook-delete-assignments.md)|None|Delete a [managedEBookAssignment](../resources/intune-managedebookassignment.md) object.|
|[Update assignments](../api/intune-iosvppebook-update-assignments.md)|[managedEBookAssignment](../resources/intune-managedebookassignment.md)|Update the properties of an assignments object.|
|[Get assignments](../api/intune-iosvppebook-get-managedebookassignment.md)|[managedEBookAssignment](../resources/intune-managedebookassignment.md)|Read the properties and relationships of a [managedEBookAssignment](../resources/intune-managedebookassignment.md) object.|
|[List installSummary](../api/intune-iosvppebook-list-installsummary.md)|[eBookInstallSummary](../resources/intune-ebookinstallsummary.md) collection|Get the eBookInstallSummaries from the installSummary navigation property.|
|[Create installSummary](../api/intune-iosvppebook-post-installsummary.md)|[eBookInstallSummary](../resources/intune-ebookinstallsummary.md)|Create a new installSummary object.|
|[Delete installSummary](../api/intune-iosvppebook-delete-installsummary.md)|None|Delete an [eBookInstallSummary](../resources/intune-ebookinstallsummary.md) object.|
|[Update installSummary](../api/intune-iosvppebook-update-installsummary.md)|[eBookInstallSummary](../resources/intune-ebookinstallsummary.md)|Update the properties of an installSummary object.|
|[Get installSummary](../api/intune-iosvppebook-get-ebookinstallsummary.md)|[eBookInstallSummary](../resources/intune-ebookinstallsummary.md)|Read the properties and relationships of an [eBookInstallSummary](../resources/intune-ebookinstallsummary.md) object.|
|[List deviceStates](../api/intune-iosvppebook-list-devicestates.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md) collection|Get the deviceInstallStates from the deviceStates navigation property.|
|[Create deviceStates](../api/intune-iosvppebook-post-devicestates.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md)|Create a new deviceStates object.|
|[Delete deviceStates](../api/intune-iosvppebook-delete-devicestates.md)|None|Delete a [deviceInstallState](../resources/intune-deviceinstallstate.md) object.|
|[Update deviceStates](../api/intune-iosvppebook-update-devicestates.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md)|Update the properties of a deviceStates object.|
|[Get deviceStates](../api/intune-iosvppebook-get-deviceinstallstate.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md)|Read the properties and relationships of a [deviceInstallState](../resources/intune-deviceinstallstate.md) object.|
|[List userStateSummary](../api/intune-iosvppebook-list-userstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md) collection|Get the userInstallStateSummaries from the userStateSummary navigation property.|
|[Create userStateSummary](../api/intune-iosvppebook-post-userstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md)|Create a new userStateSummary object.|
|[Delete userStateSummary](../api/intune-iosvppebook-delete-userstatesummary.md)|None|Delete a [userInstallStateSummary](../resources/intune-userinstallstatesummary.md) object.|
|[Update userStateSummary](../api/intune-iosvppebook-update-userstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md)|Update the properties of a userStateSummary object.|
|[Get userStateSummary](../api/intune-iosvppebook-get-userinstallstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md)|Read the properties and relationships of a [userInstallStateSummary](../resources/intune-userinstallstatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleId|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedEBook](../resources/intune-managedebook.md)|
|description|String|**TODO: Add Description** Inherited from [managedEBook](../resources/intune-managedebook.md)|
|displayName|String|**TODO: Add Description** Inherited from [managedEBook](../resources/intune-managedebook.md)|
|genres|String collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|informationUrl|String|**TODO: Add Description** Inherited from [managedEBook](../resources/intune-managedebook.md)|
|language|String|**TODO: Add Description**|
|largeCover|[mimeContent](../resources/intune-mimecontent.md)|**TODO: Add Description** Inherited from [managedEBook](../resources/intune-managedebook.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedEBook](../resources/intune-managedebook.md)|
|privacyInformationUrl|String|**TODO: Add Description** Inherited from [managedEBook](../resources/intune-managedebook.md)|
|publishedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedEBook](../resources/intune-managedebook.md)|
|publisher|String|**TODO: Add Description** Inherited from [managedEBook](../resources/intune-managedebook.md)|
|seller|String|**TODO: Add Description**|
|totalLicenseCount|Int32|**TODO: Add Description**|
|usedLicenseCount|Int32|**TODO: Add Description**|
|vppOrganizationName|String|**TODO: Add Description**|
|vppTokenId|Guid|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/intune-managedebookassignment.md) collection|**TODO: Add Description** Inherited from [managedEBook](../resources/managedebook.md)|
|deviceStates|[deviceInstallState](../resources/intune-deviceinstallstate.md) collection|**TODO: Add Description** Inherited from [managedEBook](../resources/managedebook.md)|
|installSummary|[eBookInstallSummary](../resources/intune-ebookinstallsummary.md)|**TODO: Add Description** Inherited from [managedEBook](../resources/managedebook.md)|
|userStateSummary|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md) collection|**TODO: Add Description** Inherited from [managedEBook](../resources/managedebook.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook",
  "baseType": "microsoft.graph.managedEBook",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
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
  "privacyInformationUrl": "String",
  "vppTokenId": "Guid",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": "Integer",
  "usedLicenseCount": "Integer"
}
```

