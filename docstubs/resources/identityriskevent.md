---
title: "identityRiskEvent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# identityRiskEvent resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List identityRiskEvents](../api/identityriskevent-list.md)|[identityRiskEvent](../resources/identityriskevent.md) collection|List properties and relationships of the [identityRiskEvent](../resources/identityriskevent.md) objects.|
|[Get identityRiskEvent](../api/identityriskevent-get.md)|[identityRiskEvent](../resources/identityriskevent.md)|Read properties and relationships of the [identityRiskEvent](../resources/identityriskevent.md) object.|
|[Create identityRiskEvent](../api/identityriskevent-post-identityriskevents.md)|[identityRiskEvent](../resources/identityriskevent.md)|Create a new [identityRiskEvent](../resources/identityriskevent.md) object.|
|[Delete identityRiskEvent](../api/identityriskevent-delete.md)|None|Deletes a [identityRiskEvent](../resources/identityriskevent.md).|
|[Update identityRiskEvent](../api/identityriskevent-update.md)|[identityRiskEvent](../resources/identityriskevent.md)|Update the properties of a [identityRiskEvent](../resources/identityriskevent.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|closedDateTime|DateTimeOffset||
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|riskEventDateTime|DateTimeOffset||
|riskEventStatus|Enumeration| Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskEventType|String||
|riskLevel|Enumeration| Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|userDisplayName|String||
|userId|String||
|userPrincipalName|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|impactedUser|[user](../resources/user.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityRiskEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityRiskEvent",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "riskEventDateTime": "String (timestamp)",
  "riskEventType": "String",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "userId": "String"
}
```

