---
title: "anonymousIpRiskEvent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# anonymousIpRiskEvent resource type


Namespace: microsoft.graph




Inherits from [locatedRiskEvent](../resources/locatedriskevent.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List anonymousIpRiskEvents](../api/anonymousipriskevent-list.md)|[anonymousIpRiskEvent](../resources/anonymousipriskevent.md) collection|List properties and relationships of the [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) objects.|
|[Get anonymousIpRiskEvent](../api/anonymousipriskevent-get.md)|[anonymousIpRiskEvent](../resources/anonymousipriskevent.md)|Read properties and relationships of the [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object.|
|[Create anonymousIpRiskEvent](../api/anonymousipriskevent-post-anonymousipriskevents.md)|[anonymousIpRiskEvent](../resources/anonymousipriskevent.md)|Create a new [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object.|
|[Delete anonymousIpRiskEvent](../api/anonymousipriskevent-delete.md)|None|Deletes a [anonymousIpRiskEvent](../resources/anonymousipriskevent.md).|
|[Update anonymousIpRiskEvent](../api/anonymousipriskevent-update.md)|[anonymousIpRiskEvent](../resources/anonymousipriskevent.md)|Update the properties of a [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|closedDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|createdDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|ipAddress|String| Inherited from [locatedRiskEvent](../resources/locatedriskevent.md)|
|location|[signInLocation](../resources/signinlocation.md)| Inherited from [locatedRiskEvent](../resources/locatedriskevent.md)|
|riskEventDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskEventStatus|Enumeration| Inherited from [identityRiskEvent](../resources/identityriskevent.md). Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskEventType|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskLevel|Enumeration| Inherited from [identityRiskEvent](../resources/identityriskevent.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
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

