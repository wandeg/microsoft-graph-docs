---
title: "userRegistrationCount resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# userRegistrationCount resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|registrationCount|Int64|**TODO: Add Description**|
|registrationStatus|registrationStatusType|**TODO: Add Description**. Possible values are: `registered`, `enabled`, `capable`, `mfaRegistered`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.userRegistrationCount"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.userRegistrationCount",
  "registrationStatus": "String",
  "registrationCount": 1024
}
```

