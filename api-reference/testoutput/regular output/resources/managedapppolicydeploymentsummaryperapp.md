---
title: "managedAppPolicyDeploymentSummaryPerApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedAppPolicyDeploymentSummaryPerApp resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationAppliedUserCount|Int32|Number of users the policy is applied.|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/mobileAppIdentifier.md)|Deployment of an app.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```

