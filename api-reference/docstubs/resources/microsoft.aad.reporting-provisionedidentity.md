---
title: "provisionedIdentity resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# provisionedIdentity resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|details|[detailsInfo](../resources/microsoft.aad.reporting-detailsinfo.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|identityType|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.provisionedIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "identityType": "String",
  "details": {
    "@odata.type": "Microsoft.AAD.Reporting.detailsInfo"
  }
}
```

