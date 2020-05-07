---
title: "mobileAppInstallSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileAppInstallSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32|**TODO: Add Description**|
|failedUserCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|**TODO: Add Description**|
|installedUserCount|Int32|**TODO: Add Description**|
|notApplicableDeviceCount|Int32|**TODO: Add Description**|
|notApplicableUserCount|Int32|**TODO: Add Description**|
|notInstalledDeviceCount|Int32|**TODO: Add Description**|
|notInstalledUserCount|Int32|**TODO: Add Description**|
|pendingInstallDeviceCount|Int32|**TODO: Add Description**|
|pendingInstallUserCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "notInstalledDeviceCount": "Integer",
  "pendingInstallDeviceCount": "Integer",
  "installedUserCount": "Integer",
  "failedUserCount": "Integer",
  "notApplicableUserCount": "Integer",
  "notInstalledUserCount": "Integer",
  "pendingInstallUserCount": "Integer"
}
```

