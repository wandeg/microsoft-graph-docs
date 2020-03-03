---
title: "conditionalAccessSessionControls resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# conditionalAccessSessionControls resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationEnforcedRestrictions|[applicationEnforcedRestrictionsSessionControl](../resources/applicationEnforcedRestrictionsSessionControl.md)||
|cloudAppSecurity|[cloudAppSecuritySessionControl](../resources/cloudAppSecuritySessionControl.md)||
|persistentBrowser|[persistentBrowserSessionControl](../resources/persistentBrowserSessionControl.md)||
|signInFrequency|[signInFrequencySessionControl](../resources/signInFrequencySessionControl.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessSessionControls"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessSessionControls",
  "applicationEnforcedRestrictions": {
    "@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl",
    "isEnabled": true
  },
  "cloudAppSecurity": {
    "@odata.type": "microsoft.graph.cloudAppSecuritySessionControl",
    "cloudAppSecurityType": "String"
  },
  "signInFrequency": {
    "@odata.type": "microsoft.graph.signInFrequencySessionControl",
    "value": 1024,
    "type": "String"
  },
  "persistentBrowser": {
    "@odata.type": "microsoft.graph.persistentBrowserSessionControl",
    "mode": "String"
  }
}
```

