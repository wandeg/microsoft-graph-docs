---
title: "deviceComplianceUserOverview resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceComplianceUserOverview resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceComplianceUserOverview](../api/devicecomplianceuseroverview-get.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Read the properties and relationships of a [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.|
|[Update deviceComplianceUserOverview](../api/devicecomplianceuseroverview-update.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Update the properties of a [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.|
|[List userStatusOverview](../api/devicecompliancepolicy-list-userstatusoverview.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) collection|Get the deviceComplianceUserOverviews from the userStatusOverview navigation property.|
|[Create userStatusOverview](../api/devicecompliancepolicy-post-userstatusoverview.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Create a new userStatusOverview object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationVersion|Int32|Version of the policy for that overview|
|errorCount|Int32|Number of error Users|
|failedCount|Int32|Number of failed Users|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastUpdateDateTime|DateTimeOffset|Last update time|
|notApplicableCount|Int32|Number of not applicable users|
|pendingCount|Int32|Number of pending Users|
|successCount|Int32|Number of succeeded Users|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```

