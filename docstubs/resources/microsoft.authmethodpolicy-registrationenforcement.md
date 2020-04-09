---
title: "registrationEnforcement resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# registrationEnforcement resource type


Namespace: microsoft.authMethodPolicy



## Properties
|Property|Type|Description|
|:---|:---|:---|
|isAllowedToSkipRegistration|Boolean||
|registrationSkipDurationInDays|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.authMethodPolicy.registrationEnforcement"
}
-->
``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.registrationEnforcement",
  "isAllowedToSkipRegistration": true,
  "registrationSkipDurationInDays": 1024
}
```

