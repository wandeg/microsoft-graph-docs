---
title: "hasPayloadLinkResultItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# hasPayloadLinkResultItem resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|String|Exception information indicates if check for this item was successful or not.Empty string for no error.|
|hasLink|Boolean|Indicate whether a payload has any link or not.|
|payloadId|String|Key of the Payload, In the format of Guid.|
|sources|Enumeration collection|The reason where the link comes from.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hasPayloadLinkResultItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hasPayloadLinkResultItem",
  "payloadId": "String",
  "hasLink": true,
  "error": "String",
  "sources": [
    "String"
  ]
}
```

