---
title: "policySetItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# policySetItem resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get policySetItem](../api/policysetitem-get.md)|[policySetItem](../resources/policysetitem.md)|Read properties and relationships of the [policySetItem](../resources/policysetitem.md) object.|
|[List items](../api/policyset-list-items.md)|[policySetItem](../resources/policysetitem.md) collection|Get the policySetItems from the items navigation property.|
|[Add items](../api/policyset-post-items.md)|[policySetItem](../resources/policysetitem.md)|Add items by posting to the items collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|displayName|String||
|errorCode|Enumeration| Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|itemType|String||
|lastModifiedDateTime|DateTimeOffset||
|payloadId|String||
|status|Enumeration| Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetItem",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```

