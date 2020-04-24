---
title: "governanceRoleAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# governanceRoleAssignment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List governanceRoleAssignments](../api/governanceroleassignment-list.md)|[governanceRoleAssignment](../resources/governanceroleassignment.md) collection|Get a list of the [governanceRoleAssignment](../resources/governanceroleassignment.md) objects and their properties.|
|[Get governanceRoleAssignment](../api/governanceroleassignment-get.md)|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Read the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md) object.|
|[Create governanceRoleAssignment](../api/governanceroleassignment-post-governanceroleassignments.md)|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Create a new [governanceRoleAssignment](../resources/governanceroleassignment.md) object.|
|[Delete governanceRoleAssignment](../api/governanceroleassignment-delete.md)|None|Deletes a [governanceRoleAssignment](../resources/governanceroleassignment.md) object.|
|[Update governanceRoleAssignment](../api/governanceroleassignment-update.md)|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Update the properties of a [governanceRoleAssignment](../resources/governanceroleassignment.md) object.|
|[export](../api/governanceroleassignment-export.md)|String collection|**TODO: Add Description**|
|[List resource](../api/governanceroleassignment-list-resource.md)|[governanceResource](../resources/governanceresource.md) collection|Get the governanceResources from the resource navigation property.|
|[Create resource](../api/governanceroleassignment-post-resource.md)|[governanceResource](../resources/governanceresource.md)|Create a new resource object.|
|[Delete resource](../api/governanceroleassignment-delete-resource.md)|None|Delete a [governanceResource](../resources/governanceresource.md) object.|
|[Update resource](../api/governanceroleassignment-update-resource.md)|[governanceResource](../resources/governanceresource.md)|Update the properties of a resource object.|
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceresource.md)|Read the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.|
|[List roleDefinition](../api/governanceroleassignment-list-roledefinition.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md) collection|Get the governanceRoleDefinitions from the roleDefinition navigation property.|
|[Create roleDefinition](../api/governanceroleassignment-post-roledefinition.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Create a new roleDefinition object.|
|[Delete roleDefinition](../api/governanceroleassignment-delete-roledefinition.md)|None|Delete a [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Update roleDefinition](../api/governanceroleassignment-update-roledefinition.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Update the properties of a roleDefinition object.|
|[Get governanceRoleDefinition](../api/governanceroledefinition-get.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Read the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[List subject](../api/governanceroleassignment-list-subject.md)|[governanceSubject](../resources/governancesubject.md) collection|Get the governanceSubjects from the subject navigation property.|
|[Create subject](../api/governanceroleassignment-post-subject.md)|[governanceSubject](../resources/governancesubject.md)|Create a new subject object.|
|[Delete subject](../api/governanceroleassignment-delete-subject.md)|None|Delete a [governanceSubject](../resources/governancesubject.md) object.|
|[Update subject](../api/governanceroleassignment-update-subject.md)|[governanceSubject](../resources/governancesubject.md)|Update the properties of a subject object.|
|[Get governanceSubject](../api/governancesubject-get.md)|[governanceSubject](../resources/governancesubject.md)|Read the properties and relationships of a [governanceSubject](../resources/governancesubject.md) object.|
|[List linkedEligibleRoleAssignment](../api/governanceroleassignment-list-linkedeligibleroleassignment.md)|[governanceRoleAssignment](../resources/governanceroleassignment.md) collection|Get the governanceRoleAssignments from the linkedEligibleRoleAssignment navigation property.|
|[Add linkedEligibleRoleAssignment](../api/governanceroleassignment-post-linkedeligibleroleassignment.md)|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Add linkedEligibleRoleAssignment by posting to the linkedEligibleRoleAssignment collection.|
|[Remove linkedEligibleRoleAssignment](../api/governanceroleassignment-delete-linkedeligibleroleassignment.md)|None|Remove a [governanceRoleAssignment](../resources/governanceroleassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentState|String|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|linkedEligibleRoleAssignmentId|String|**TODO: Add Description**|
|memberType|String|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|roleDefinitionId|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|subjectId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|**TODO: Add Description**|
|resource|[governanceResource](../resources/governanceresource.md)|**TODO: Add Description**|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|**TODO: Add Description**|
|subject|[governanceSubject](../resources/governancesubject.md)|**TODO: Add Description**|

## JSON representation
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

