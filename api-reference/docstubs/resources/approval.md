---
title: "approval resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# approval resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get approval](../api/approval-get.md)|[approval](../resources/approval.md)|Read properties and relationships of an [approval](../resources/approval.md) object.|
|[Update approval](../api/approval-update.md)|[approval](../resources/approval.md)|Update the properties of a [approval](../resources/approval.md) object.|
|[List pendingSteps](../api/approval-list-pendingsteps.md)|[approvalStep](../resources/approvalstep.md) collection|Get the approvalSteps from the pendingSteps navigation property.|
|[Create pendingSteps](../api/approval-post-pendingsteps.md)|[approvalStep](../resources/approvalstep.md)|Create a new pendingSteps object.|
|[Delete pendingSteps](../api/approval-delete-pendingsteps.md)|None|Delete a pendingSteps object.|
|[Update pendingSteps](../api/approval-update-pendingsteps.md)|[approvalStep](../resources/approvalstep.md)|Update the properties of a pendingSteps object.|
|[Get approvalStep](../api/approvalstep-get.md)|[approvalStep](../resources/approvalstep.md)|Read properties and relationships of an [approvalStep](../resources/approvalstep.md) object.|
|[List completedSteps](../api/approval-list-completedsteps.md)|[approvalStep](../resources/approvalstep.md) collection|Get the approvalSteps from the completedSteps navigation property.|
|[Create completedSteps](../api/approval-post-completedsteps.md)|[approvalStep](../resources/approvalstep.md)|Create a new completedSteps object.|
|[Delete completedSteps](../api/approval-delete-completedsteps.md)|None|Delete a completedSteps object.|
|[Update completedSteps](../api/approval-update-completedsteps.md)|[approvalStep](../resources/approvalstep.md)|Update the properties of a completedSteps object.|
|[Get approvalStep](../api/approvalstep-get.md)|[approvalStep](../resources/approvalstep.md)|Read properties and relationships of an [approvalStep](../resources/approvalstep.md) object.|
|[List request](../api/approval-list-request.md)|[request](../resources/request.md) collection|Get the requests from the request navigation property.|
|[Add request](../api/approval-post-request.md)|[request](../resources/request.md)|Add request by posting to the request collection.|
|[Remove request](../api/approval-delete-request.md)|None|Remove a request object.|
|[List approval](../api/userconsentrequest-list-approval.md)|[approval](../resources/approval.md) collection|Get the approvals from the approval navigation property.|
|[Create approval](../api/userconsentrequest-post-approval.md)|[approval](../resources/approval.md)|Create a new approval object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|completedSteps|[approvalStep](../resources/approvalstep.md) collection|**TODO: Add Description**|
|pendingSteps|[approvalStep](../resources/approvalstep.md) collection|**TODO: Add Description**|
|request|[request](../resources/request.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)"
}
```

