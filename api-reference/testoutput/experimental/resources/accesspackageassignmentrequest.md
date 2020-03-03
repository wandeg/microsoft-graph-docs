---
title: "accessPackageAssignmentRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# accessPackageAssignmentRequest resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md)|[accessPackageAssignmentRequest](../resources/accessPackageAssignmentRequest.md)|Read properties and relationships of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[Delete accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md)|None|Deletes a [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).|
|[Update accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-update.md)|[accessPackageAssignmentRequest](../resources/accessPackageAssignmentRequest.md)|Update the properties of a [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[My](../api/accesspackageassignmentrequest-my.md)|[accessPackageAssignmentRequest](../resources/accessPackageAssignmentRequest.md) collection||
|[Cancel](../api/accesspackageassignmentrequest-cancel.md)|None||
|[Get accessPackage](../api/accesspackage-get.md)|[accessPackage](../resources/accessPackage.md)|Read properties and relationships of the [accessPackage](../resources/accesspackage.md) object.|
|[Get accessPackageAssignment](../api/accesspackageassignment-get.md)|[accessPackageAssignment](../resources/accessPackageAssignment.md)|Read properties and relationships of the [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[Get accessPackageSubject](../api/accesspackagesubject-get.md)|[accessPackageSubject](../resources/accessPackageSubject.md)|Read properties and relationships of the [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[List accessPackageAssignmentRequests](../api/accesspackageassignment-list-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accessPackageAssignmentRequest.md) collection|Get the accessPackageAssignmentRequests from the accessPackageAssignmentRequests navigation property.|
|[Add accessPackageAssignmentRequests](../api/accesspackageassignment-post-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accessPackageAssignmentRequest.md)|Add accessPackageAssignmentRequests by posting to the accessPackageAssignmentRequests collection.|

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
|accessPackage|[accessPackage](../resources/accessPackage.md)||
|accessPackageAssignment|[accessPackageAssignment](../resources/accessPackageAssignment.md)||
|requestor|[accessPackageSubject](../resources/accessPackageSubject.md)||

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

