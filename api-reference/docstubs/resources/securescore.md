---
title: "secureScore resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# secureScore resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get secureScore](../api/securescore-get.md)|[secureScore](../resources/securescore.md)|Read the properties and relationships of a [secureScore](../resources/securescore.md) object.|
|[Update secureScore](../api/securescore-update.md)|[secureScore](../resources/securescore.md)|Update the properties of a [secureScore](../resources/securescore.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeUserCount|Int32|**TODO: Add Description**|
|averageComparativeScores|[averageComparativeScore](../resources/averagecomparativescore.md) collection|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|controlScores|[controlScore](../resources/controlscore.md) collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|currentScore|Double|**TODO: Add Description**|
|enabledServices|String collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|licensedUserCount|Int32|**TODO: Add Description**|
|maxScore|Double|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

