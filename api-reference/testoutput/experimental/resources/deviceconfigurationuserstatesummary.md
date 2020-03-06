---
title: "deviceConfigurationUserStateSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationUserStateSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfigurationUserStateSummary](../api/deviceconfigurationuserstatesummary-get.md)|[deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md)|Read properties and relationships of the [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) object.|
|[Update deviceConfigurationUserStateSummary](../api/deviceconfigurationuserstatesummary-update.md)|[deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md)|Update the properties of a [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantUserCount|Int32|Number of compliant users|
|conflictUserCount|Int32|Number of conflict users|
|errorUserCount|Int32|Number of error users|
|id|String| Inherited from [entity](../resources/entity.md)|
|nonCompliantUserCount|Int32|Number of NonCompliant users|
|notApplicableUserCount|Int32|Number of not applicable users|
|remediatedUserCount|Int32|Number of remediated users|
|unknownUserCount|Int32|Number of unknown users|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "String (identifier)",
  "unknownUserCount": 1024,
  "notApplicableUserCount": 1024,
  "compliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "errorUserCount": 1024,
  "conflictUserCount": 1024
}
```

