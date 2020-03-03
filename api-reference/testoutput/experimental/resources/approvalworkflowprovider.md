---
title: "approvalWorkflowProvider resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# approvalWorkflowProvider resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List approvalWorkflowProviders](../api/approvalworkflowprovider-list.md)|[approvalWorkflowProvider](../resources/approvalWorkflowProvider.md) collection|List properties and relationships of the [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) objects.|
|[Get approvalWorkflowProvider](../api/approvalworkflowprovider-get.md)|[approvalWorkflowProvider](../resources/approvalWorkflowProvider.md)|Read properties and relationships of the [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object.|
|[Create approvalWorkflowProvider](../api/approvalworkflowprovider-post-approvalworkflowproviders.md)|[approvalWorkflowProvider](../resources/approvalWorkflowProvider.md)|Create a new [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object.|
|[Delete approvalWorkflowProvider](../api/approvalworkflowprovider-delete.md)|None|Deletes a [approvalWorkflowProvider](../resources/approvalworkflowprovider.md).|
|[Update approvalWorkflowProvider](../api/approvalworkflowprovider-update.md)|[approvalWorkflowProvider](../resources/approvalWorkflowProvider.md)|Update the properties of a [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object.|
|[List businessFlows](../api/approvalworkflowprovider-list-businessflows.md)|[businessFlow](../resources/businessFlow.md) collection|Get the businessFlows from the businessFlows navigation property.|
|[Add businessFlows](../api/approvalworkflowprovider-post-businessflows.md)|[businessFlow](../resources/businessFlow.md)|Add businessFlows by posting to the businessFlows collection.|
|[List policyTemplates](../api/approvalworkflowprovider-list-policytemplates.md)|[governancePolicyTemplate](../resources/governancePolicyTemplate.md) collection|Get the governancePolicyTemplates from the policyTemplates navigation property.|
|[Add policyTemplates](../api/approvalworkflowprovider-post-policytemplates.md)|[governancePolicyTemplate](../resources/governancePolicyTemplate.md)|Add policyTemplates by posting to the policyTemplates collection.|
|[List requests](../api/approvalworkflowprovider-list-requests.md)|[request](../resources/request.md) collection|Get the requests from the requests navigation property.|
|[Add requests](../api/approvalworkflowprovider-post-requests.md)|[request](../resources/request.md)|Add requests by posting to the requests collection.|
|[List requestsAwaitingMyDecision](../api/approvalworkflowprovider-list-requestsawaitingmydecision.md)|[request](../resources/request.md) collection|Get the requests from the requestsAwaitingMyDecision navigation property.|
|[Add requestsAwaitingMyDecision](../api/approvalworkflowprovider-post-requestsawaitingmydecision.md)|[request](../resources/request.md)|Add requestsAwaitingMyDecision by posting to the requestsAwaitingMyDecision collection.|
|[List businessFlowsWithRequestsAwaitingMyDecision](../api/approvalworkflowprovider-list-businessflowswithrequestsawaitingmydecision.md)|[businessFlow](../resources/businessFlow.md) collection|Get the businessFlows from the businessFlowsWithRequestsAwaitingMyDecision navigation property.|
|[Add businessFlowsWithRequestsAwaitingMyDecision](../api/approvalworkflowprovider-post-businessflowswithrequestsawaitingmydecision.md)|[businessFlow](../resources/businessFlow.md)|Add businessFlowsWithRequestsAwaitingMyDecision by posting to the businessFlowsWithRequestsAwaitingMyDecision collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|businessFlows|[businessFlow](../resources/businessFlow.md) collection||
|businessFlowsWithRequestsAwaitingMyDecision|[businessFlow](../resources/businessFlow.md) collection||
|policyTemplates|[governancePolicyTemplate](../resources/governancePolicyTemplate.md) collection||
|requests|[request](../resources/request.md) collection||
|requestsAwaitingMyDecision|[request](../resources/request.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalWorkflowProvider",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approvalWorkflowProvider",
  "id": "String (identifier)",
  "displayName": "String"
}
```

