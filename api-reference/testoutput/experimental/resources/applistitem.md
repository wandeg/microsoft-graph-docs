---
title: "appListItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# appListItem resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String|The application or bundle identifier of the application|
|appStoreUrl|String|The Store URL of the application|
|name|String|The application name|
|publisher|String|The publisher of the application|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```

