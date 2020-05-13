---
title: "appFamilyDetails resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appFamilyDetails resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|groupDisplayName|String|**TODO: Add Description**|
|groupId|String|**TODO: Add Description**|
|status|appFamilyLinkedInStatus|**TODO: Add Description**. Possible values are: `OptOut`, `OptIn`, `NotProvisioned`, `OptIn_Selected`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appFamilyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appFamilyDetails",
  "status": "String",
  "groupDisplayName": "String",
  "groupId": "String"
}
```

