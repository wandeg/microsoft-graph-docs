---
title: "governanceRoleAssignmentRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# governanceRoleAssignmentRequest resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List governanceRoleAssignmentRequests](../api/governanceroleassignmentrequest-list.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection|Get a list of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects and their properties.|
|[Get governanceRoleAssignmentRequest](../api/governanceroleassignmentrequest-get.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Read the properties and relationships of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.|
|[Create governanceRoleAssignmentRequest](../api/governanceroleassignmentrequest-post-governanceroleassignmentrequests.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Create a new [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.|
|[Delete governanceRoleAssignmentRequest](../api/governanceroleassignmentrequest-delete.md)|None|Deletes a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.|
|[Update governanceRoleAssignmentRequest](../api/governanceroleassignmentrequest-update.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Update the properties of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.|
|[cancel](../api/governanceroleassignmentrequest-cancel.md)|None|**TODO: Add Description**|
|[updateRequest](../api/governanceroleassignmentrequest-updaterequest.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|**TODO: Add Description**|
|[List resource](../api/governanceroleassignmentrequest-list-resource.md)|[governanceResource](../resources/governanceresource.md) collection|Get the governanceResources from the resource navigation property.|
|[Create resource](../api/governanceroleassignmentrequest-post-resource.md)|[governanceResource](../resources/governanceresource.md)|Create a new resource object.|
|[Delete resource](../api/governanceroleassignmentrequest-delete-resource.md)|None|Delete a [governanceResource](../resources/governanceresource.md) object.|
|[Update resource](../api/governanceroleassignmentrequest-update-resource.md)|[governanceResource](../resources/governanceresource.md)|Update the properties of a resource object.|
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceresource.md)|Read the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.|
|[List roleDefinition](../api/governanceroleassignmentrequest-list-roledefinition.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md) collection|Get the governanceRoleDefinitions from the roleDefinition navigation property.|
|[Create roleDefinition](../api/governanceroleassignmentrequest-post-roledefinition.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Create a new roleDefinition object.|
|[Delete roleDefinition](../api/governanceroleassignmentrequest-delete-roledefinition.md)|None|Delete a [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Update roleDefinition](../api/governanceroleassignmentrequest-update-roledefinition.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Update the properties of a roleDefinition object.|
|[Get governanceRoleDefinition](../api/governanceroledefinition-get.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Read the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[List subject](../api/governanceroleassignmentrequest-list-subject.md)|[governanceSubject](../resources/governancesubject.md) collection|Get the governanceSubjects from the subject navigation property.|
|[Create subject](../api/governanceroleassignmentrequest-post-subject.md)|[governanceSubject](../resources/governancesubject.md)|Create a new subject object.|
|[Delete subject](../api/governanceroleassignmentrequest-delete-subject.md)|None|Delete a [governanceSubject](../resources/governancesubject.md) object.|
|[Update subject](../api/governanceroleassignmentrequest-update-subject.md)|[governanceSubject](../resources/governancesubject.md)|Update the properties of a subject object.|
|[Get governanceSubject](../api/governancesubject-get.md)|[governanceSubject](../resources/governancesubject.md)|Read the properties and relationships of a [governanceSubject](../resources/governancesubject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentState|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|linkedEligibleRoleAssignmentId|String|**TODO: Add Description**|
|reason|String|**TODO: Add Description**|
|requestedDateTime|DateTimeOffset|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|roleDefinitionId|String|**TODO: Add Description**|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|**TODO: Add Description**|
|status|[governanceRoleAssignmentRequestStatus](../resources/governanceroleassignmentrequeststatus.md)|**TODO: Add Description**|
|subjectId|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[governanceResource](../resources/governanceresource.md)|**TODO: Add Description**|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|**TODO: Add Description**|
|subject|[governanceSubject](../resources/governancesubject.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "type": "String",
  "assignmentState": "String",
  "requestedDateTime": "String (timestamp)",
  "reason": "String",
  "status": {
    "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus",
    "status": "String",
    "subStatus": "String",
    "statusDetails": [
      {
        "@odata.type": "microsoft.graph.keyValue",
        "key": "String",
        "value": "String"
      }
    ]
  },
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule",
    "startDateTime": "String (timestamp)",
    "endDateTime": "String (timestamp)",
    "duration": "String (duration)"
  }
}
```

