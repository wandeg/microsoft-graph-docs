---
title: "targetResource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# targetResource resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|groupType|groupType|**TODO: Add Description**. Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.|
|id|String|**TODO: Add Description**|
|modifiedProperties|[modifiedProperty](../resources/microsoft.aad.reporting-modifiedproperty.md) collection|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

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

