---
title: "workforceIntegration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workforceIntegration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [changeTrackedEntity](../resources/changetrackedentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workforceIntegration](../api/workforceintegration-get.md)|[workforceIntegration](../resources/workforceintegration.md)|Read the properties and relationships of a [workforceIntegration](../resources/workforceintegration.md) object.|
|[Update workforceIntegration](../api/workforceintegration-update.md)|[workforceIntegration](../resources/workforceintegration.md)|Update the properties of a [workforceIntegration](../resources/workforceintegration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|apiVersion|Int32|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|displayName|String|**TODO: Add Description**|
|eligibilityFilteringEnabledEntities|eligibilityFilteringEnabledEntities|**TODO: Add Description**. Possible values are: `none`, `swapRequest`, `offerShiftRequest`, `unknownFutureValue`.|
|encryption|[workforceIntegrationEncryption](../resources/workforceintegrationencryption.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isActive|Boolean|**TODO: Add Description**|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|supportedEntities|workforceIntegrationSupportedEntities|**TODO: Add Description**. Possible values are: `none`, `shift`, `swapRequest`, `userShiftPreferences`, `openShift`, `openShiftRequest`, `offerShiftRequest`, `unknownFutureValue`.|
|supports|workforceIntegrationSupportedEntities|**TODO: Add Description**. Possible values are: `none`, `shift`, `swapRequest`, `userShiftPreferences`, `openShift`, `openShiftRequest`, `offerShiftRequest`, `unknownFutureValue`.|
|url|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workforceIntegration",
  "baseType": "microsoft.graph.changeTrackedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workforceIntegration",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "displayName": "String",
  "apiVersion": 1024,
  "encryption": {
    "@odata.type": "microsoft.graph.workforceIntegrationEncryption"
  },
  "isActive": true,
  "url": "String",
  "supports": "String",
  "supportedEntities": "String",
  "eligibilityFilteringEnabledEntities": "String"
}
```

