---
title: "FlagContentRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# FlagContentRequest resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentUrn|String||
|flaggingReason|Enumeration| Possible values are: `ADVERTISEMENT`, `COPYRIGHT`, `PORNOGRAPHIC`, `INAPPROPRIATE_CONTENT`, `SPAM_CONTENT`, `INAPPROPRIATE_PICTURE`, `MISREPRESENTATION`, `OUT_OF_DATE`, `PLAGIARISM`, `OTHER`, `IRRELEVANT`, `PROMOTION`, `GRATUITOUSLY_SHOCKING`, `HARASSMENT`, `THREATS_OF_VIOLENCE`, `ACCOUNT_HACKED`, `OFFENSIVE`, `IMPERSONATION`, `FAKE_IDENTITY`, `FAKE_CONTENT`, `SUICIDAL`, `INACCURATE_MEMBER_INFORMATION`, `DECEASED`, `SEEN_OFTEN`, `BROKEN_LINKS`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.FlagContentRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.FlagContentRequest",
  "contentUrn": "String",
  "flaggingReason": "String"
}
```

