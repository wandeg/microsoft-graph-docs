---
title: "accessPackageAssignmentRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageAssignmentRequest resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection|Get a list of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects and their properties.|
|[Get accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Read the properties and relationships of an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[Create accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[Delete accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md)|None|Deletes an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[Update accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-update.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Update the properties of an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[My](../api/accesspackageassignmentrequest-my.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection|**TODO: Add Description**|
|[Cancel](../api/accesspackageassignmentrequest-cancel.md)|None|**TODO: Add Description**|
|[List accessPackage](../api/accesspackageassignmentrequest-list-accesspackage.md)|[accessPackage](../resources/accesspackage.md) collection|Get the accessPackages from the accessPackage navigation property.|
|[Add accessPackage](../api/accesspackageassignmentrequest-post-accesspackage.md)|[accessPackage](../resources/accesspackage.md)|Add accessPackage by posting to the accessPackage collection.|
|[Remove accessPackage](../api/accesspackageassignmentrequest-delete-accesspackage.md)|None|Remove an [accessPackage](../resources/accesspackage.md) object.|
|[List accessPackageAssignment](../api/accesspackageassignmentrequest-list-accesspackageassignment.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) collection|Get the accessPackageAssignments from the accessPackageAssignment navigation property.|
|[Create accessPackageAssignment](../api/accesspackageassignmentrequest-post-accesspackageassignment.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Create a new accessPackageAssignment object.|
|[Delete accessPackageAssignment](../api/accesspackageassignmentrequest-delete-accesspackageassignment.md)|None|Delete an [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[Update accessPackageAssignment](../api/accesspackageassignmentrequest-update-accesspackageassignment.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Update the properties of an accessPackageAssignment object.|
|[Get accessPackageAssignment](../api/accesspackageassignment-get.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Read the properties and relationships of an [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[List requestor](../api/accesspackageassignmentrequest-list-requestor.md)|[accessPackageSubject](../resources/accesspackagesubject.md) collection|Get the accessPackageSubjects from the requestor navigation property.|
|[Create requestor](../api/accesspackageassignmentrequest-post-requestor.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Create a new requestor object.|
|[Delete requestor](../api/accesspackageassignmentrequest-delete-requestor.md)|None|Delete a [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[Update requestor](../api/accesspackageassignmentrequest-update-requestor.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Update the properties of a requestor object.|
|[Get accessPackageSubject](../api/accesspackagesubject-get.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Read the properties and relationships of an [accessPackageSubject](../resources/accesspackagesubject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDate|DateTimeOffset|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isValidationOnly|Boolean|**TODO: Add Description**|
|justification|String|**TODO: Add Description**|
|requestState|String|**TODO: Add Description**|
|requestStatus|String|**TODO: Add Description**|
|requestType|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|**TODO: Add Description**|
|accessPackageAssignment|[accessPackageAssignment](../resources/accesspackageassignment.md)|**TODO: Add Description**|
|requestor|[accessPackageSubject](../resources/accesspackagesubject.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "id": "String (identifier)",
  "requestType": "String",
  "requestState": "String",
  "requestStatus": "String",
  "isValidationOnly": true,
  "createdDateTime": "String (timestamp)",
  "completedDate": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "justification": "String"
}
```

