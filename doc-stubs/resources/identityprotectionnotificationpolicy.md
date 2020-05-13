---
title: "identityProtectionNotificationPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# identityProtectionNotificationPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userAlertsSettings|[userAlertsSettings](../resources/useralertssettings.md)|**TODO: Add Description**|
|weeklyDigestSettings|[weeklyDigestSettings](../resources/weeklydigestsettings.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityProtectionNotificationPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityProtectionNotificationPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "weeklyDigestSettings": {
    "@odata.type": "microsoft.graph.weeklyDigestSettings"
  },
  "userAlertsSettings": {
    "@odata.type": "microsoft.graph.userAlertsSettings"
  }
}
```

