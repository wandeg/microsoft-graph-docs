---
title: "approvalWorkflowProvider resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# approvalWorkflowProvider resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List approvalWorkflowProviders](../api/approvalworkflowprovider-list.md)|[approvalWorkflowProvider](../resources/approvalworkflowprovider.md) collection|Get a list of the [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) objects and their properties.|
|[Get approvalWorkflowProvider](../api/approvalworkflowprovider-get.md)|[approvalWorkflowProvider](../resources/approvalworkflowprovider.md)|Read properties and relationships of an [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object.|
|[Create approvalWorkflowProvider](../api/approvalworkflowprovider-post-approvalworkflowproviders.md)|[approvalWorkflowProvider](../resources/approvalworkflowprovider.md)|Create a new [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object.|
|[Delete approvalWorkflowProvider](../api/approvalworkflowprovider-delete.md)|None|Deletes an [approvalWorkflowProvider](../resources/approvalworkflowprovider.md).|
|[Update approvalWorkflowProvider](../api/approvalworkflowprovider-update.md)|[approvalWorkflowProvider](../resources/approvalworkflowprovider.md)|Update the properties of a [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object.|
|[List businessFlows](../api/approvalworkflowprovider-list-businessflows.md)|[businessFlow](../resources/businessflow.md) collection|Get the businessFlows from the businessFlows navigation property.|
|[Create businessFlows](../api/approvalworkflowprovider-post-businessflows.md)|[businessFlow](../resources/businessflow.md)|Create a new businessFlows object.|
|[Delete businessFlows](../api/approvalworkflowprovider-delete-businessflows.md)|None|Delete a businessFlows object.|
|[Update businessFlows](../api/approvalworkflowprovider-update-businessflows.md)|[businessFlow](../resources/businessflow.md)|Update the properties of a businessFlows object.|
|[Get businessFlow](../api/businessflow-get.md)|[businessFlow](../resources/businessflow.md)|Read properties and relationships of a [businessFlow](../resources/businessflow.md) object.|
|[List policyTemplates](../api/approvalworkflowprovider-list-policytemplates.md)|[governancePolicyTemplate](../resources/governancepolicytemplate.md) collection|Get the governancePolicyTemplates from the policyTemplates navigation property.|
|[Create policyTemplates](../api/approvalworkflowprovider-post-policytemplates.md)|[governancePolicyTemplate](../resources/governancepolicytemplate.md)|Create a new policyTemplates object.|
|[Delete policyTemplates](../api/approvalworkflowprovider-delete-policytemplates.md)|None|Delete a policyTemplates object.|
|[Update policyTemplates](../api/approvalworkflowprovider-update-policytemplates.md)|[governancePolicyTemplate](../resources/governancepolicytemplate.md)|Update the properties of a policyTemplates object.|
|[Get governancePolicyTemplate](../api/governancepolicytemplate-get.md)|[governancePolicyTemplate](../resources/governancepolicytemplate.md)|Read properties and relationships of a [governancePolicyTemplate](../resources/governancepolicytemplate.md) object.|
|[List businessFlowsWithRequestsAwaitingMyDecision](../api/approvalworkflowprovider-list-businessflowswithrequestsawaitingmydecision.md)|[businessFlow](../resources/businessflow.md) collection|Get the businessFlows from the businessFlowsWithRequestsAwaitingMyDecision navigation property.|
|[Create businessFlowsWithRequestsAwaitingMyDecision](../api/approvalworkflowprovider-post-businessflowswithrequestsawaitingmydecision.md)|[businessFlow](../resources/businessflow.md)|Create a new businessFlowsWithRequestsAwaitingMyDecision object.|
|[Delete businessFlowsWithRequestsAwaitingMyDecision](../api/approvalworkflowprovider-delete-businessflowswithrequestsawaitingmydecision.md)|None|Delete a businessFlowsWithRequestsAwaitingMyDecision object.|
|[Update businessFlowsWithRequestsAwaitingMyDecision](../api/approvalworkflowprovider-update-businessflowswithrequestsawaitingmydecision.md)|[businessFlow](../resources/businessflow.md)|Update the properties of a businessFlowsWithRequestsAwaitingMyDecision object.|
|[Get businessFlow](../api/businessflow-get.md)|[businessFlow](../resources/businessflow.md)|Read properties and relationships of a [businessFlow](../resources/businessflow.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|businessFlows|[businessFlow](../resources/businessflow.md) collection|**TODO: Add Description**|
|businessFlowsWithRequestsAwaitingMyDecision|[businessFlow](../resources/businessflow.md) collection|**TODO: Add Description**|
|policyTemplates|[governancePolicyTemplate](../resources/governancepolicytemplate.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalWorkflowProvider",
  "baseType": "",
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

