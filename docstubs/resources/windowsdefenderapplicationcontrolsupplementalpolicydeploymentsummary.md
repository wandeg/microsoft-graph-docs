---
title: "windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.|
|[Update windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-update.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deployedDeviceCount|Int32||
|failedDeviceCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|

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

