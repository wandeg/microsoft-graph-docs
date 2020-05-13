---
title: "softwareUpdateStatusSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# softwareUpdateStatusSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|**TODO: Add Description**|
|compliantUserCount|Int32|**TODO: Add Description**|
|conflictDeviceCount|Int32|**TODO: Add Description**|
|conflictUserCount|Int32|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|errorDeviceCount|Int32|**TODO: Add Description**|
|errorUserCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|nonCompliantDeviceCount|Int32|**TODO: Add Description**|
|nonCompliantUserCount|Int32|**TODO: Add Description**|
|notApplicableDeviceCount|Int32|**TODO: Add Description**|
|notApplicableUserCount|Int32|**TODO: Add Description**|
|remediatedDeviceCount|Int32|**TODO: Add Description**|
|remediatedUserCount|Int32|**TODO: Add Description**|
|unknownDeviceCount|Int32|**TODO: Add Description**|
|unknownUserCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": "Integer",
  "nonCompliantDeviceCount": "Integer",
  "remediatedDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "unknownDeviceCount": "Integer",
  "conflictDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "compliantUserCount": "Integer",
  "nonCompliantUserCount": "Integer",
  "remediatedUserCount": "Integer",
  "errorUserCount": "Integer",
  "unknownUserCount": "Integer",
  "conflictUserCount": "Integer",
  "notApplicableUserCount": "Integer"
}
```

