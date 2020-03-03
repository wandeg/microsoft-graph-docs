---
title: "unfamiliarLocationRiskEvent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# unfamiliarLocationRiskEvent resource type




Inherits from [locatedRiskEvent](../resources/locatedRiskEvent.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List unfamiliarLocationRiskEvents](../api/unfamiliarlocationriskevent-list.md)|[unfamiliarLocationRiskEvent](../resources/unfamiliarLocationRiskEvent.md) collection|List properties and relationships of the [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) objects.|
|[Get unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md)|[unfamiliarLocationRiskEvent](../resources/unfamiliarLocationRiskEvent.md)|Read properties and relationships of the [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object.|
|[Create unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-post-unfamiliarlocationriskevents.md)|[unfamiliarLocationRiskEvent](../resources/unfamiliarLocationRiskEvent.md)|Create a new [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object.|
|[Delete unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-delete.md)|None|Deletes a [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md).|
|[Update unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-update.md)|[unfamiliarLocationRiskEvent](../resources/unfamiliarLocationRiskEvent.md)|Update the properties of a [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|closedDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|createdDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|ipAddress|String| Inherited from [locatedRiskEvent](../resources/locatedRiskEvent.md)|
|location|[signInLocation](../resources/signInLocation.md)| Inherited from [locatedRiskEvent](../resources/locatedRiskEvent.md)|
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
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent",
  "baseType": "microsoft.graph.locatedRiskEvent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "riskEventDateTime": "String (timestamp)",
  "riskEventType": "String",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "userId": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation",
    "countryOrRegion": "String",
    "geoCoordinates": {
      "@odata.type": "microsoft.graph.geoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double"
    }
  },
  "ipAddress": "String"
}
```

