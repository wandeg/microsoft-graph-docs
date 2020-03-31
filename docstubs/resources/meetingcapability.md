---
title: "meetingCapability resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# meetingCapability resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowAnonymousUsersToDialOut|Boolean||
|allowAnonymousUsersToStartMeeting|Boolean||
|autoAdmittedUsers|Enumeration| Possible values are: `everyoneInCompany`, `everyone`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingCapability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingCapability",
  "allowAnonymousUsersToDialOut": true,
  "autoAdmittedUsers": "String",
  "allowAnonymousUsersToStartMeeting": true
}
```

