---
title: "configurationManagerClientInformation resource type"
description: "Configuration Manager client information synced from SCCM"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# configurationManagerClientInformation resource type


Namespace: microsoft.graph

Configuration Manager client information synced from SCCM

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientIdentifier|String|Configuration Manager Client Id from SCCM|
|isBlocked|Boolean|Configuration Manager Client blocked status from SCCM|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.configurationManagerClientInformation",
  "clientIdentifier": "String",
  "isBlocked": "Boolean"
}
```

