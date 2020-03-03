---
title: "workforceIntegration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workforceIntegration resource type




Inherits from [changeTrackedEntity](../resources/changeTrackedEntity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workforceIntegrations](../api/workforceintegration-list.md)|[workforceIntegration](../resources/workforceIntegration.md) collection|List properties and relationships of the [workforceIntegration](../resources/workforceintegration.md) objects.|
|[Get workforceIntegration](../api/workforceintegration-get.md)|[workforceIntegration](../resources/workforceIntegration.md)|Read properties and relationships of the [workforceIntegration](../resources/workforceintegration.md) object.|
|[Create workforceIntegration](../api/workforceintegration-create.md)|[workforceIntegration](../resources/workforceIntegration.md)|Create a new [workforceIntegration](../resources/workforceintegration.md) object.|
|[Delete workforceIntegration](../api/workforceintegration-delete.md)|None|Deletes a [workforceIntegration](../resources/workforceintegration.md).|
|[Update workforceIntegration](../api/workforceintegration-update.md)|[workforceIntegration](../resources/workforceIntegration.md)|Update the properties of a [workforceIntegration](../resources/workforceintegration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|apiVersion|Int32||
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|displayName|String||
|encryption|[workforceIntegrationEncryption](../resources/workforceIntegrationEncryption.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|isActive|Boolean||
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|supports|Enumeration|. Possible values are: `none`, `shift`, `swapRequest`, `userShiftPreferences`, `openShift`, `openShiftRequest`, `offerShiftRequest`, `unknownFutureValue`.|
|url|String||

## Relationships
None

## JSON Representation
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
  "supports": "String"
}
```

