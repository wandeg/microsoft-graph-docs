---
title: "relyingPartyDetailedSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# relyingPartyDetailedSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List relyingPartyDetailedSummaries](../api/relyingpartydetailedsummary-list.md)|[relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) collection|List properties and relationships of the [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) objects.|
|[Get relyingPartyDetailedSummary](../api/relyingpartydetailedsummary-get.md)|[relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md)|Read properties and relationships of the [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object.|
|[Create relyingPartyDetailedSummary](../api/relyingpartydetailedsummary-create.md)|[relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md)|Create a new [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object.|
|[Delete relyingPartyDetailedSummary](../api/relyingpartydetailedsummary-delete.md)|None|Deletes a [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md).|
|[Update relyingPartyDetailedSummary](../api/relyingpartydetailedsummary-update.md)|[relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md)|Update the properties of a [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedSignInCount|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|migrationStatus|Enumeration|. Possible values are: `ready`, `needsReview`, `additionalStepsRequired`, `unknownFutureValue`.|
|migrationValidationDetails|[keyValuePair](../resources/keyvaluepair.md) collection||
|relyingPartyId|String||
|relyingPartyName|String||
|replyUrls|String collection||
|serviceId|String||
|signInSuccessRate|Double||
|successfulSignInCount|Int64||
|totalSignInCount|Int64||
|uniqueUserCount|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.relyingPartyDetailedSummary",
  "id": "String (identifier)",
  "relyingPartyId": "String",
  "serviceId": "String",
  "relyingPartyName": "String",
  "successfulSignInCount": 1024,
  "failedSignInCount": 1024,
  "totalSignInCount": 1024,
  "signInSuccessRate": "Double",
  "uniqueUserCount": 1024,
  "migrationStatus": "String",
  "migrationValidationDetails": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "replyUrls": [
    "String"
  ]
}
```

