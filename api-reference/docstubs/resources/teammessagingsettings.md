---
title: "teamMessagingSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# teamMessagingSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowChannelMentions|Boolean|**TODO: Add Description**|
|allowOwnerDeleteMessages|Boolean|**TODO: Add Description**|
|allowTeamMentions|Boolean|**TODO: Add Description**|
|allowUserDeleteMessages|Boolean|**TODO: Add Description**|
|allowUserEditMessages|Boolean|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamMessagingSettings",
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true
}
```

