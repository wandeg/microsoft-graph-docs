---
title: "securityAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# securityAction resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get securityAction](../api/securityaction-get.md)|[securityAction](../resources/securityaction.md)|Read properties and relationships of the [securityAction](../resources/securityaction.md) object.|
|[Update securityAction](../api/securityaction-update.md)|[securityAction](../resources/securityaction.md)|Update the properties of a [securityAction](../resources/securityaction.md) object.|
|[cancelSecurityAction](../api/securityaction-cancelsecurityaction.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionReason|String||
|appId|String||
|azureTenantId|String||
|clientContext|String||
|completedDateTime|DateTimeOffset||
|createdDateTime|DateTimeOffset||
|errorInfo|[ResultInfo](../resources/resultinfo.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastActionDateTime|DateTimeOffset||
|name|String||
|parameters|[keyValuePair](../resources/keyvaluepair.md) collection||
|states|[securityActionState](../resources/securityactionstate.md) collection||
|status|Enumeration|. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|user|String||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityAction",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityAction",
  "id": "String (identifier)",
  "actionReason": "String",
  "appId": "String",
  "azureTenantId": "String",
  "clientContext": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "errorInfo": {
    "@odata.type": "microsoft.graph.ResultInfo"
  },
  "lastActionDateTime": "String (timestamp)",
  "name": "String",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "states": [
    {
      "@odata.type": "microsoft.graph.securityActionState"
    }
  ],
  "status": "String",
  "user": "String",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```

