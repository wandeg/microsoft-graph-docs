---
title: "windowsDefenderApplicationControlSupplementalPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsDefenderApplicationControlSupplementalPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[assign](../api/windowsdefenderapplicationcontrolsupplementalpolicy-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/windowsdefenderapplicationcontrolsupplementalpolicy-list-assignments.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) collection|Get the windowsDefenderApplicationControlSupplementalPolicyAssignments from the assignments navigation property.|
|[Create assignments](../api/windowsdefenderapplicationcontrolsupplementalpolicy-post-assignments.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/windowsdefenderapplicationcontrolsupplementalpolicy-delete-assignments.md)|None|Delete an [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.|
|[Update assignments](../api/windowsdefenderapplicationcontrolsupplementalpolicy-update-assignments.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Update the properties of an assignments object.|
|[Get windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/windowsdefenderapplicationcontrolsupplementalpolicyassignment-get.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Read the properties and relationships of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.|
|[List deploySummary](../api/windowsdefenderapplicationcontrolsupplementalpolicy-list-deploysummary.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) collection|Get the windowsDefenderApplicationControlSupplementalPolicyDeploymentSummaries from the deploySummary navigation property.|
|[Create deploySummary](../api/windowsdefenderapplicationcontrolsupplementalpolicy-post-deploysummary.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Create a new deploySummary object.|
|[Delete deploySummary](../api/windowsdefenderapplicationcontrolsupplementalpolicy-delete-deploysummary.md)|None|Delete a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.|
|[Update deploySummary](../api/windowsdefenderapplicationcontrolsupplementalpolicy-update-deploysummary.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Update the properties of a deploySummary object.|
|[Get windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Read the properties and relationships of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.|
|[List deviceStatuses](../api/windowsdefenderapplicationcontrolsupplementalpolicy-list-devicestatuses.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) collection|Get the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus from the deviceStatuses navigation property.|
|[Create deviceStatuses](../api/windowsdefenderapplicationcontrolsupplementalpolicy-post-devicestatuses.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Create a new deviceStatuses object.|
|[Delete deviceStatuses](../api/windowsdefenderapplicationcontrolsupplementalpolicy-delete-devicestatuses.md)|None|Delete a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.|
|[Update deviceStatuses](../api/windowsdefenderapplicationcontrolsupplementalpolicy-update-devicestatuses.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Update the properties of a deviceStatuses object.|
|[Get windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Read the properties and relationships of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Binary|**TODO: Add Description**|
|contentFileName|String|**TODO: Add Description**|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|version|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) collection|**TODO: Add Description**|
|deploySummary|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|**TODO: Add Description**|
|deviceStatuses|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "content": "Binary",
  "contentFileName": "String",
  "version": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```

