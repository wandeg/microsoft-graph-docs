---
title: "governanceRoleAssignmentRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# governanceRoleAssignmentRequest resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List governanceRoleAssignmentRequests](../api/governanceroleassignmentrequest-list.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection|List properties and relationships of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects.|
|[Get governanceRoleAssignmentRequest](../api/governanceroleassignmentrequest-get.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Read properties and relationships of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.|
|[Create governanceRoleAssignmentRequest](../api/governanceroleassignmentrequest-post-governanceroleassignmentrequests.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Create a new [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.|
|[Delete governanceRoleAssignmentRequest](../api/governanceroleassignmentrequest-delete.md)|None|Deletes a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).|
|[Update governanceRoleAssignmentRequest](../api/governanceroleassignmentrequest-update.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Update the properties of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.|
|[cancel](../api/governanceroleassignmentrequest-cancel.md)|None||
|[updateRequest](../api/governanceroleassignmentrequest-updaterequest.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)||
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceresource.md)|Read properties and relationships of the [governanceResource](../resources/governanceresource.md) object.|
|[Get governanceRoleDefinition](../api/governanceroledefinition-get.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Read properties and relationships of the [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Get governanceSubject](../api/governancesubject-get.md)|[governanceSubject](../resources/governancesubject.md)|Read properties and relationships of the [governanceSubject](../resources/governancesubject.md) object.|

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
|schedule|[governanceSchedule](../resources/governanceschedule.md)||
|status|[governanceRoleAssignmentRequestStatus](../resources/governanceroleassignmentrequeststatus.md)||
|subjectId|String||
|type|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[governanceResource](../resources/governanceresource.md)||
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)||
|subject|[governanceSubject](../resources/governancesubject.md)||

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

