---
title: "androidForWorkAppConfigurationSchemaItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidForWorkAppConfigurationSchemaItem resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|dataType|Enumeration|The type of value this item describes. Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.|
|defaultBoolValue|Boolean|Default value for boolean type items, if specified by the app developer|
|defaultIntValue|Int32|Default value for integer type items, if specified by the app developer|
|defaultStringArrayValue|String collection|Default value for string array type items, if specified by the app developer|
|defaultStringValue|String|Default value for string type items, if specified by the app developer|
|description|String|Description of what the item controls within the application|
|displayName|String|Human readable name|
|schemaItemKey|String|Unique key the application uses to identify the item|
|selections|[keyValuePair](../resources/keyvaluepair.md) collection|List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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

