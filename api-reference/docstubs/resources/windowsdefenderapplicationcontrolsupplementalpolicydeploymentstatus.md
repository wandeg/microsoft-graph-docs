---
title: "windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus resource type"
description: "Contains properties for the deployment state of a WindowsDefenderApplicationControl supplemental policy for a device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus resource type


Namespace: microsoft.graph

Contains properties for the deployment state of a WindowsDefenderApplicationControl supplemental policy for a device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Read the properties and relationships of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.|
|[Update windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-update.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.|
|[List policy](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-list-policy.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) collection|Get the windowsDefenderApplicationControlSupplementalPolicies from the policy navigation property.|
|[Add policy](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-post-policy.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md)|Add policy by posting to the policy collection.|
|[Remove policy](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-delete-policy.md)|None|Remove a [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deploymentStatus|windowsDefenderApplicationControlSupplementalPolicyStatuses|The deployment state of the policy. Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.|
|deviceId|String|Device ID.|
|deviceName|String|Device name.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|Last sync date time.|
|osDescription|String|Windows OS Version Description.|
|osVersion|String|Windows OS Version.|
|policyVersion|String|Human readable version of the WindowsDefenderApplicationControl supplemental policy.|
|userName|String|The name of the user of this device.|
|userPrincipalName|String|User Principal Name.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|policy|[windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md)|The navigation link to the WindowsDefenderApplicationControl supplemental policy.|

## JSON representation
Here is a JSON representation of the resource.
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

