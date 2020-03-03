---
title: "accessPackageAssignmentRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackageAssignmentRequest resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection|List properties and relationships of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.|
|[Get accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Read properties and relationships of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[Create accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[Delete accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md)|None|Deletes a [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).|
|[Update accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-update.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Update the properties of a [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[My](../api/accesspackageassignmentrequest-my.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection||
|[Cancel](../api/accesspackageassignmentrequest-cancel.md)|None||
|[Get accessPackage](../api/accesspackage-get.md)|[accessPackage](../resources/accesspackage.md)|Read properties and relationships of the [accessPackage](../resources/accesspackage.md) object.|
|[Get accessPackageAssignment](../api/accesspackageassignment-get.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Read properties and relationships of the [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[Get accessPackageSubject](../api/accesspackagesubject-get.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Read properties and relationships of the [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[List accessPackageAssignmentRequests](../api/accesspackageassignment-list-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection|Get the accessPackageAssignmentRequests from the accessPackageAssignmentRequests navigation property.|
|[Add accessPackageAssignmentRequests](../api/accesspackageassignment-post-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Add accessPackageAssignmentRequests by posting to the accessPackageAssignmentRequests collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDate|DateTimeOffset||
|createdDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|isValidationOnly|Boolean||
|justification|String||
|requestState|String||
|requestStatus|String||
|requestType|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)||
|accessPackageAssignment|[accessPackageAssignment](../resources/accesspackageassignment.md)||
|requestor|[accessPackageSubject](../resources/accesspackagesubject.md)||

## JSON Representation
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

