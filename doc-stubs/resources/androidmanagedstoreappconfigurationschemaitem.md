---
title: "androidManagedStoreAppConfigurationSchemaItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# androidManagedStoreAppConfigurationSchemaItem resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|dataType|androidManagedStoreAppConfigurationSchemaItemDataType|**TODO: Add Description**. Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.|
|defaultBoolValue|Boolean|**TODO: Add Description**|
|defaultIntValue|Int32|**TODO: Add Description**|
|defaultStringArrayValue|String collection|**TODO: Add Description**|
|defaultStringValue|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|index|Int32|**TODO: Add Description**|
|parentIndex|Int32|**TODO: Add Description**|
|schemaItemKey|String|**TODO: Add Description**|
|selections|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
  "index": "Integer",
  "parentIndex": "Integer",
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": "Boolean",
  "defaultIntValue": "Integer",
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```

