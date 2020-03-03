---
title: "policySetItem resource type"
description: "A class containing the properties used for PolicySet Item."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# policySetItem resource type


Namespace: microsoft.graph

A class containing the properties used for PolicySet Item.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List policySetItems](../api/policysetitem-list.md)|[policySetItem](../resources/policysetitem.md) collection|List properties and relationships of the [policySetItem](../resources/policysetitem.md) objects.|
|[Get policySetItem](../api/policysetitem-get.md)|[policySetItem](../resources/policysetitem.md)|Read properties and relationships of the [policySetItem](../resources/policysetitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Creation time of the PolicySetItem.|
|displayName|String|DisplayName of the PolicySetItem.|
|errorCode|Enumeration|Error code if any occured. Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Tags of the guided deployment|
|id|String| Inherited from [entity](../resources/entity.md)|
|itemType|String|policySetType of the PolicySetItem.|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySetItem.|
|payloadId|String|PayloadId of the PolicySetItem.|
|status|Enumeration|Status of the PolicySetItem. Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|

## Relationships
None

## JSON Representation
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

