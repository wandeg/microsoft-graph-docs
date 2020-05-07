---
title: "windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List policy](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-list-policy.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) collection|Get the windowsDefenderApplicationControlSupplementalPolicies from the policy navigation property.|
|[Add policy](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-post-policy.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md)|Add policy by posting to the policy collection.|
|[Remove policy](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-delete-policy.md)|None|Remove a [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object.|
|[List deviceStatuses](../api/windowsdefenderapplicationcontrolsupplementalpolicy-list-devicestatuses.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) collection|Get the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus from the deviceStatuses navigation property.|
|[Create deviceStatuses](../api/windowsdefenderapplicationcontrolsupplementalpolicy-post-devicestatuses.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Create a new deviceStatuses object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deploymentStatus|windowsDefenderApplicationControlSupplementalPolicyStatuses|**TODO: Add Description**. Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.|
|deviceId|String|**TODO: Add Description**|
|deviceName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|osDescription|String|**TODO: Add Description**|
|osVersion|String|**TODO: Add Description**|
|policyVersion|String|**TODO: Add Description**|
|userName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|policy|[windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "osVersion": "String",
  "osDescription": "String",
  "deploymentStatus": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "policyVersion": "String"
}
```

