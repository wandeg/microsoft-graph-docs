---
title: "provisioningSystemDetails resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# provisioningSystemDetails resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|details|[detailsInfo](../resources/microsoft.aad.reporting-detailsinfo.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.provisioningSystemDetails",
  "id": "String (identifier)",
  "displayName": "String",
  "details": {
    "@odata.type": "Microsoft.AAD.Reporting.detailsInfo"
  }
}
```

