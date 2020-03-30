---
title: "managedAppPolicyDeploymentSummaryPerApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedAppPolicyDeploymentSummaryPerApp resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationAppliedUserCount|Int32||
|mobileAppIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)||

## Relationships
None

## JSON representation
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

