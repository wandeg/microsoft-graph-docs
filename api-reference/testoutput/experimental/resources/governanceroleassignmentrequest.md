---
title: "governanceRoleAssignmentRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# governanceRoleAssignmentRequest resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get governanceRoleAssignmentRequest](../api/governanceroleassignmentrequest-get.md)|[governanceRoleAssignmentRequest](../resources/governanceRoleAssignmentRequest.md)|Read properties and relationships of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.|
|[Delete governanceRoleAssignmentRequest](../api/governanceroleassignmentrequest-delete.md)|None|Deletes a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).|
|[Update governanceRoleAssignmentRequest](../api/governanceroleassignmentrequest-update.md)|[governanceRoleAssignmentRequest](../resources/governanceRoleAssignmentRequest.md)|Update the properties of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.|
|[cancel](../api/governanceroleassignmentrequest-cancel.md)|None||
|[updateRequest](../api/governanceroleassignmentrequest-updaterequest.md)|[governanceRoleAssignmentRequest](../resources/governanceRoleAssignmentRequest.md)||
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceResource.md)|Read properties and relationships of the [governanceResource](../resources/governanceresource.md) object.|
|[Get governanceRoleDefinition](../api/governanceroledefinition-get.md)|[governanceRoleDefinition](../resources/governanceRoleDefinition.md)|Read properties and relationships of the [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Get governanceSubject](../api/governancesubject-get.md)|[governanceSubject](../resources/governanceSubject.md)|Read properties and relationships of the [governanceSubject](../resources/governancesubject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentState|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|linkedEligibleRoleAssignmentId|String||
|reason|String||
|requestedDateTime|DateTimeOffset||
|resourceId|String||
|roleDefinitionId|String||
|schedule|[governanceSchedule](../resources/governanceSchedule.md)||
|status|[governanceRoleAssignmentRequestStatus](../resources/governanceRoleAssignmentRequestStatus.md)||
|subjectId|String||
|type|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[governanceResource](../resources/governanceResource.md)||
|roleDefinition|[governanceRoleDefinition](../resources/governanceRoleDefinition.md)||
|subject|[governanceSubject](../resources/governanceSubject.md)||

## JSON Representation
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

