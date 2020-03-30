---
title: "impossibleTravelRiskEvent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# impossibleTravelRiskEvent resource type


Namespace: microsoft.graph




Inherits from [locatedRiskEvent](../resources/locatedriskevent.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List impossibleTravelRiskEvents](../api/impossibletravelriskevent-list.md)|[impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) collection|List properties and relationships of the [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) objects.|
|[Get impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md)|[impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md)|Read properties and relationships of the [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object.|
|[Create impossibleTravelRiskEvent](../api/impossibletravelriskevent-post-impossibletravelriskevents.md)|[impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md)|Create a new [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object.|
|[Delete impossibleTravelRiskEvent](../api/impossibletravelriskevent-delete.md)|None|Deletes a [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md).|
|[Update impossibleTravelRiskEvent](../api/impossibletravelriskevent-update.md)|[impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md)|Update the properties of a [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|closedDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|createdDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|deviceInformation|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|ipAddress|String| Inherited from [locatedRiskEvent](../resources/locatedriskevent.md)|
|isAtypicalLocation|Boolean||
|location|[signInLocation](../resources/signinlocation.md)| Inherited from [locatedRiskEvent](../resources/locatedriskevent.md)|
|previousIpAddress|String||
|previousLocation|[signInLocation](../resources/signinlocation.md)||
|previousSigninDateTime|DateTimeOffset||
|riskEventDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskEventStatus|Enumeration| Inherited from [identityRiskEvent](../resources/identityriskevent.md). Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskEventType|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskLevel|Enumeration| Inherited from [identityRiskEvent](../resources/identityriskevent.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|userAgent|String||
|userDisplayName|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|userId|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|userPrincipalName|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|impactedUser|[user](../resources/user.md)| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|

## JSON representation
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

