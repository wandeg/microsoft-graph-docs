---
title: "windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.|
|[Update windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-update.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.|
|[Get windowsDefenderApplicationControlSupplementalPolicy](../api/windowsdefenderapplicationcontrolsupplementalpolicy-get.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md)|Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deploymentStatus|Enumeration| Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.|
|deviceId|String||
|deviceName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset||
|osDescription|String||
|osVersion|String||
|policyVersion|String||
|userName|String||
|userPrincipalName|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|policy|[windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md)||

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

