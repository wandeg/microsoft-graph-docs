---
title: "typedEmailAddress resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# typedEmailAddress resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [emailAddress](../resources/emailaddress.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String|**TODO: Add Description** Inherited from [emailAddress](../resources/emailaddress.md)|
|name|String|**TODO: Add Description** Inherited from [emailAddress](../resources/emailaddress.md)|
|otherLabel|String|**TODO: Add Description**|
|type|emailType|**TODO: Add Description**. Possible values are: `unknown`, `work`, `personal`, `main`, `other`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.typedEmailAddress"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.typedEmailAddress",
  "name": "String",
  "address": "String",
  "type": "String",
  "otherLabel": "String"
}
```

