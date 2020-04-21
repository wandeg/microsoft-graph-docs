---
title: "security resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# security resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get security](../api/security-get.md)|[security](../resources/security.md)|Read properties and relationships of a [security](../resources/security.md) object.|
|[Update security](../api/security-update.md)|[security](../resources/security.md)|Update the properties of a [security](../resources/security.md) object.|
|[List alerts](../api/security-list-alerts.md)|[alert](../resources/alert.md) collection|Get the alerts from the alerts navigation property.|
|[Create alerts](../api/security-post-alerts.md)|[alert](../resources/alert.md)|Create a new alerts object.|
|[Delete alerts](../api/security-delete-alerts.md)|None|Delete an alerts object.|
|[Update alerts](../api/security-update-alerts.md)|[alert](../resources/alert.md)|Update the properties of an alerts object.|
|[Get alert](../api/alert-get.md)|[alert](../resources/alert.md)|Read properties and relationships of an [alert](../resources/alert.md) object.|
|[List secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md) collection|Get the secureScoreControlProfiles from the secureScoreControlProfiles navigation property.|
|[Create secureScoreControlProfiles](../api/security-post-securescorecontrolprofiles.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md)|Create a new secureScoreControlProfiles object.|
|[Delete secureScoreControlProfiles](../api/security-delete-securescorecontrolprofiles.md)|None|Delete a secureScoreControlProfiles object.|
|[Update secureScoreControlProfiles](../api/security-update-securescorecontrolprofiles.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md)|Update the properties of a secureScoreControlProfiles object.|
|[Get secureScoreControlProfile](../api/securescorecontrolprofile-get.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md)|Read properties and relationships of a [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.|
|[List secureScores](../api/security-list-securescores.md)|[secureScore](../resources/securescore.md) collection|Get the secureScores from the secureScores navigation property.|
|[Create secureScores](../api/security-post-securescores.md)|[secureScore](../resources/securescore.md)|Create a new secureScores object.|
|[Delete secureScores](../api/security-delete-securescores.md)|None|Delete a secureScores object.|
|[Update secureScores](../api/security-update-securescores.md)|[secureScore](../resources/securescore.md)|Update the properties of a secureScores object.|
|[Get secureScore](../api/securescore-get.md)|[secureScore](../resources/securescore.md)|Read properties and relationships of a [secureScore](../resources/securescore.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|alerts|[alert](../resources/alert.md) collection|**TODO: Add Description**|
|secureScoreControlProfiles|[secureScoreControlProfile](../resources/securescorecontrolprofile.md) collection|**TODO: Add Description**|
|secureScores|[secureScore](../resources/securescore.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security",
  "id": "String (identifier)"
}
```

