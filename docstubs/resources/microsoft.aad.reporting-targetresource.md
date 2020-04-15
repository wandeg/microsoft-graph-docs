---
title: "targetResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# targetResource resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|groupType|Enumeration| Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.|
|id|String||
|modifiedProperties|[modifiedProperty](../resources/microsoft.aad.reporting-modifiedproperty.md) collection||
|type|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.targetResource"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.targetResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String",
  "modifiedProperties": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.modifiedProperty",
      "oldValue": "String",
      "newValue": "String"
    }
  ]
}
```

