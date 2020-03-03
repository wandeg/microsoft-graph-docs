---
title: "leakedCredentialsRiskEvent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# leakedCredentialsRiskEvent resource type




Inherits from [identityRiskEvent](../resources/identityRiskEvent.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List leakedCredentialsRiskEvents](../api/leakedcredentialsriskevent-list.md)|[leakedCredentialsRiskEvent](../resources/leakedCredentialsRiskEvent.md) collection|List properties and relationships of the [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) objects.|
|[Get leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md)|[leakedCredentialsRiskEvent](../resources/leakedCredentialsRiskEvent.md)|Read properties and relationships of the [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object.|
|[Create leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-post-leakedcredentialsriskevents.md)|[leakedCredentialsRiskEvent](../resources/leakedCredentialsRiskEvent.md)|Create a new [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object.|
|[Delete leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-delete.md)|None|Deletes a [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md).|
|[Update leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-update.md)|[leakedCredentialsRiskEvent](../resources/leakedCredentialsRiskEvent.md)|Update the properties of a [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|closedDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|createdDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|riskEventDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|riskEventStatus|Enumeration| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md). Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskEventType|String| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|riskLevel|Enumeration| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|userDisplayName|String| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|userId|String| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|userPrincipalName|String| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|impactedUser|[user](../resources/user.md)| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent",
  "baseType": "microsoft.graph.identityRiskEvent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.leakedCredentialsRiskEvent",
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

