---
title: "conditionalAccessSessionControls resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# conditionalAccessSessionControls resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationEnforcedRestrictions|[applicationEnforcedRestrictionsSessionControl](../resources/applicationenforcedrestrictionssessioncontrol.md)||
|cloudAppSecurity|[cloudAppSecuritySessionControl](../resources/cloudappsecuritysessioncontrol.md)||
|persistentBrowser|[persistentBrowserSessionControl](../resources/persistentbrowsersessioncontrol.md)||
|signInFrequency|[signInFrequencySessionControl](../resources/signinfrequencysessioncontrol.md)||

## Relationships
None

## JSON representation
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

