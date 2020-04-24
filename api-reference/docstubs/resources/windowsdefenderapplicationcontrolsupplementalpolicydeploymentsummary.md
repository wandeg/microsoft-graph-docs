---
title: "windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary resource type"
description: "Contains properties for the deployment summary of a WindowsDefenderApplicationControl supplemental policy."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary resource type


Namespace: microsoft.graph

Contains properties for the deployment summary of a WindowsDefenderApplicationControl supplemental policy.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Read the properties and relationships of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.|
|[Update windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-update.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deployedDeviceCount|Int32|Number of Devices that have successfully deployed this WindowsDefenderApplicationControl supplemental policy.|
|failedDeviceCount|Int32|Number of Devices that have failed to deploy this WindowsDefenderApplicationControl supplemental policy.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
  "id": "String (identifier)",
  "deployedDeviceCount": 1024,
  "failedDeviceCount": 1024
}
```

