---
title: "windowsDefenderApplicationControlSupplementalPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsDefenderApplicationControlSupplementalPolicy resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsDefenderApplicationControlSupplementalPolicy](../api/windowsdefenderapplicationcontrolsupplementalpolicy-get.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md)|Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object.|
|[Update windowsDefenderApplicationControlSupplementalPolicy](../api/windowsdefenderapplicationcontrolsupplementalpolicy-update.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md)|Update the properties of a [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object.|
|[assign](../api/windowsdefenderapplicationcontrolsupplementalpolicy-assign.md)|None||
|[List assignments](../api/windowsdefenderapplicationcontrolsupplementalpolicy-list-assignments.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) collection|Get the windowsDefenderApplicationControlSupplementalPolicyAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsdefenderapplicationcontrolsupplementalpolicy-post-assignments.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Add assignments by posting to the assignments collection.|
|[Get windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.|
|[List deviceStatuses](../api/windowsdefenderapplicationcontrolsupplementalpolicy-list-devicestatuses.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) collection|Get the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/windowsdefenderapplicationcontrolsupplementalpolicy-post-devicestatuses.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Binary|The WindowsDefenderApplicationControl supplemental policy content in byte array format.|
|contentFileName|String|The WindowsDefenderApplicationControl supplemental policy content's file name.|
|creationDateTime|DateTimeOffset|The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.|
|description|String|The description of WindowsDefenderApplicationControl supplemental policy.|
|displayName|String|The display name of WindowsDefenderApplicationControl supplemental policy.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.|
|roleScopeTagIds|String collection|List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.|
|version|String|The WindowsDefenderApplicationControl supplemental policy's version.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) collection|The associated group assignments for this WindowsDefenderApplicationControl supplemental policy.|
|deploySummary|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|WindowsDefenderApplicationControl supplemental policy deployment summary.|
|deviceStatuses|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) collection|The list of device deployment states for this WindowsDefenderApplicationControl supplemental policy.|

## JSON representation
Here is a JSON representation of the resource.
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
  "content": "binary",
  "contentFileName": "String",
  "version": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```

