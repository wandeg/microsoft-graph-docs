---
title: "sharedAppleDeviceUser resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# sharedAppleDeviceUser resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|dataQuota|Int64|Data quota|
|dataToSync|Boolean|Data to sync|
|dataUsed|Int64|Data quota|
|userPrincipalName|String|User name|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": "Boolean",
  "dataQuota": "Integer",
  "dataUsed": "Integer"
}
```

