---
title: "automaticRepliesSetting resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# automaticRepliesSetting resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|externalAudience|Enumeration|. Possible values are: `none`, `contactsOnly`, `all`.|
|externalReplyMessage|String||
|internalReplyMessage|String||
|scheduledEndDateTime|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||
|scheduledStartDateTime|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||
|status|Enumeration|. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.|

## Relationships
None

## JSON Representation
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
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "String",
    "timeZone": "String"
  },
  "scheduledEndDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "internalReplyMessage": "String",
  "externalReplyMessage": "String"
}
```

