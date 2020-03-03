---
title: "anonymousIpRiskEvent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# anonymousIpRiskEvent resource type




Inherits from [locatedRiskEvent](../resources/locatedRiskEvent.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List anonymousIpRiskEvents](../api/anonymousipriskevent-list.md)|[anonymousIpRiskEvent](../resources/anonymousIpRiskEvent.md) collection|List properties and relationships of the [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) objects.|
|[Get anonymousIpRiskEvent](../api/anonymousipriskevent-get.md)|[anonymousIpRiskEvent](../resources/anonymousIpRiskEvent.md)|Read properties and relationships of the [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object.|
|[Create anonymousIpRiskEvent](../api/anonymousipriskevent-post-anonymousipriskevents.md)|[anonymousIpRiskEvent](../resources/anonymousIpRiskEvent.md)|Create a new [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object.|
|[Delete anonymousIpRiskEvent](../api/anonymousipriskevent-delete.md)|None|Deletes a [anonymousIpRiskEvent](../resources/anonymousipriskevent.md).|
|[Update anonymousIpRiskEvent](../api/anonymousipriskevent-update.md)|[anonymousIpRiskEvent](../resources/anonymousIpRiskEvent.md)|Update the properties of a [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object.|
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
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent",
  "baseType": "microsoft.graph.locatedRiskEvent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.anonymousIpRiskEvent",
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

