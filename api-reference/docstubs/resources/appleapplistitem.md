---
title: "appleAppListItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appleAppListItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [appListItem](../resources/applistitem.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String|The bundle identifier of the application Inherited from [appListItem](../resources/applistitem.md)|
|appStoreUrl|String|The Store URL of the application Inherited from [appListItem](../resources/applistitem.md)|
|name|String|The application name Inherited from [appListItem](../resources/applistitem.md)|
|publisher|String|The publisher of the application Inherited from [appListItem](../resources/applistitem.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleAppListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleAppListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```

