---
title: "configurationManagerClientEnabledFeatures resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# configurationManagerClientEnabledFeatures resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliancePolicy|Boolean||
|deviceConfiguration|Boolean||
|endpointProtection|Boolean||
|inventory|Boolean||
|modernApps|Boolean||
|officeApps|Boolean||
|resourceAccess|Boolean||
|windowsUpdateForBusiness|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true,
  "endpointProtection": true,
  "officeApps": true
}
```

