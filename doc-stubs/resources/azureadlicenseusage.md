---
title: "azureADLicenseUsage resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# azureADLicenseUsage resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|licenseInfoDetails|[licenseInfoDetail](../resources/licenseinfodetail.md) collection|**TODO: Add Description**|
|snapshotDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.azureADLicenseUsage",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureADLicenseUsage",
  "id": "String (identifier)",
  "snapshotDateTime": "String (timestamp)",
  "licenseInfoDetails": [
    {
      "@odata.type": "microsoft.graph.licenseInfoDetail"
    }
  ]
}
```

