---
title: "impossibleTravelRiskEvent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# impossibleTravelRiskEvent resource type




Inherits from [locatedRiskEvent](../resources/locatedRiskEvent.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List impossibleTravelRiskEvents](../api/impossibletravelriskevent-list.md)|[impossibleTravelRiskEvent](../resources/impossibleTravelRiskEvent.md) collection|List properties and relationships of the [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) objects.|
|[Get impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md)|[impossibleTravelRiskEvent](../resources/impossibleTravelRiskEvent.md)|Read properties and relationships of the [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object.|
|[Create impossibleTravelRiskEvent](../api/impossibletravelriskevent-post-impossibletravelriskevents.md)|[impossibleTravelRiskEvent](../resources/impossibleTravelRiskEvent.md)|Create a new [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object.|
|[Delete impossibleTravelRiskEvent](../api/impossibletravelriskevent-delete.md)|None|Deletes a [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md).|
|[Update impossibleTravelRiskEvent](../api/impossibletravelriskevent-update.md)|[impossibleTravelRiskEvent](../resources/impossibleTravelRiskEvent.md)|Update the properties of a [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|closedDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|createdDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|deviceInformation|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|ipAddress|String| Inherited from [locatedRiskEvent](../resources/locatedRiskEvent.md)|
|isAtypicalLocation|Boolean||
|location|[signInLocation](../resources/signInLocation.md)| Inherited from [locatedRiskEvent](../resources/locatedRiskEvent.md)|
|previousIpAddress|String||
|previousLocation|[signInLocation](../resources/signInLocation.md)||
|previousSigninDateTime|DateTimeOffset||
|riskEventDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|riskEventStatus|Enumeration| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md). Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskEventType|String| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md)|
|riskLevel|Enumeration| Inherited from [identityRiskEvent](../resources/identityRiskEvent.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|userAgent|String||
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
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent",
  "baseType": "microsoft.graph.locatedRiskEvent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
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
  "ipAddress": "String",
  "userAgent": "String",
  "deviceInformation": "String",
  "isAtypicalLocation": true,
  "previousSigninDateTime": "String (timestamp)",
  "previousLocation": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "previousIpAddress": "String"
}
```

