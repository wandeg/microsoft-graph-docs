---
title: "secureScore resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# secureScore resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get secureScore](../api/securescore-get.md)|[secureScore](../resources/secureScore.md)|Read properties and relationships of the [secureScore](../resources/securescore.md) object.|
|[Delete secureScore](../api/securescore-delete.md)|None|Deletes a [secureScore](../resources/securescore.md).|
|[Update secureScore](../api/securescore-update.md)|[secureScore](../resources/secureScore.md)|Update the properties of a [secureScore](../resources/securescore.md) object.|
|[List secureScores](../api/security-list-securescores.md)|[secureScore](../resources/secureScore.md) collection|Get the secureScores from the secureScores navigation property.|
|[Add secureScores](../api/security-post-securescores.md)|[secureScore](../resources/secureScore.md)|Add secureScores by posting to the secureScores collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeUserCount|Int32||
|averageComparativeScores|[averageComparativeScore](../resources/averageComparativeScore.md) collection||
|azureTenantId|String||
|controlScores|[controlScore](../resources/controlScore.md) collection||
|createdDateTime|DateTimeOffset||
|currentScore|Double||
|enabledServices|String collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|licensedUserCount|Int32||
|maxScore|Double||
|vendorInformation|[securityVendorInformation](../resources/securityVendorInformation.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.secureScore",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.secureScore",
  "id": "String (identifier)",
  "activeUserCount": 1024,
  "averageComparativeScores": [
    {
      "@odata.type": "microsoft.graph.averageComparativeScore"
    }
  ],
  "azureTenantId": "String",
  "controlScores": [
    {
      "@odata.type": "microsoft.graph.controlScore"
    }
  ],
  "createdDateTime": "String (timestamp)",
  "currentScore": "Double",
  "enabledServices": [
    "String"
  ],
  "licensedUserCount": 1024,
  "maxScore": "Double",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```

