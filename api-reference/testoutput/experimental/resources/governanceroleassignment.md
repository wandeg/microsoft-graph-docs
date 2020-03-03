---
title: "governanceRoleAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# governanceRoleAssignment resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get governanceRoleAssignment](../api/governanceroleassignment-get.md)|[governanceRoleAssignment](../resources/governanceRoleAssignment.md)|Read properties and relationships of the [governanceRoleAssignment](../resources/governanceroleassignment.md) object.|
|[Delete governanceRoleAssignment](../api/governanceroleassignment-delete.md)|None|Deletes a [governanceRoleAssignment](../resources/governanceroleassignment.md).|
|[Update governanceRoleAssignment](../api/governanceroleassignment-update.md)|[governanceRoleAssignment](../resources/governanceRoleAssignment.md)|Update the properties of a [governanceRoleAssignment](../resources/governanceroleassignment.md) object.|
|[export](../api/governanceroleassignment-export.md)|String collection||
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceResource.md)|Read properties and relationships of the [governanceResource](../resources/governanceresource.md) object.|
|[Get governanceRoleDefinition](../api/governanceroledefinition-get.md)|[governanceRoleDefinition](../resources/governanceRoleDefinition.md)|Read properties and relationships of the [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Get governanceSubject](../api/governancesubject-get.md)|[governanceSubject](../resources/governanceSubject.md)|Read properties and relationships of the [governanceSubject](../resources/governancesubject.md) object.|
|[Get governanceRoleAssignment](../api/governanceroleassignment-get.md)|[governanceRoleAssignment](../resources/governanceRoleAssignment.md)|Read properties and relationships of the [governanceRoleAssignment](../resources/governanceroleassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentState|String||
|endDateTime|DateTimeOffset||
|externalId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|linkedEligibleRoleAssignmentId|String||
|memberType|String||
|resourceId|String||
|roleDefinitionId|String||
|startDateTime|DateTimeOffset||
|status|String||
|subjectId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceRoleAssignment.md)||
|resource|[governanceResource](../resources/governanceResource.md)||
|roleDefinition|[governanceRoleDefinition](../resources/governanceRoleDefinition.md)||
|subject|[governanceSubject](../resources/governanceSubject.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.governanceRoleAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceRoleAssignment",
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "memberType": "String",
  "assignmentState": "String",
  "status": "String"
}
```

