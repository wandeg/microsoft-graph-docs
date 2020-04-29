---
title: "automaticRepliesSetting resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# automaticRepliesSetting resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|externalAudience|externalAudienceScope|**TODO: Add Description**. Possible values are: `none`, `contactsOnly`, `all`.|
|externalReplyMessage|String|**TODO: Add Description**|
|internalReplyMessage|String|**TODO: Add Description**|
|scheduledEndDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|scheduledStartDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|status|automaticRepliesStatus|**TODO: Add Description**. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.|

## Relationships
None.

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.automaticRepliesSetting",
  "status": "String",
  "externalAudience": "String",
  "scheduledStartDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "scheduledEndDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "internalReplyMessage": "String",
  "externalReplyMessage": "String"
}
```

