---
title: "androidManagedStoreAppConfigurationSchemaItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidManagedStoreAppConfigurationSchemaItem resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|dataType|Enumeration| Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.|
|defaultBoolValue|Boolean||
|defaultIntValue|Int32||
|defaultStringArrayValue|String collection||
|defaultStringValue|String||
|description|String||
|displayName|String||
|index|Int32||
|parentIndex|Int32||
|schemaItemKey|String||
|selections|[keyValuePair](../resources/keyvaluepair.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
  "index": 1024,
  "parentIndex": 1024,
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```

