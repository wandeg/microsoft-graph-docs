---
title: "FlagContentRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# FlagContentRequest resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentUrn|String|**TODO: Add Description**|
|flaggingReason|UserReportedFlagReason|**TODO: Add Description**. Possible values are: `ADVERTISEMENT`, `COPYRIGHT`, `PORNOGRAPHIC`, `INAPPROPRIATE_CONTENT`, `SPAM_CONTENT`, `INAPPROPRIATE_PICTURE`, `MISREPRESENTATION`, `OUT_OF_DATE`, `PLAGIARISM`, `OTHER`, `IRRELEVANT`, `PROMOTION`, `GRATUITOUSLY_SHOCKING`, `HARASSMENT`, `THREATS_OF_VIOLENCE`, `ACCOUNT_HACKED`, `OFFENSIVE`, `IMPERSONATION`, `FAKE_IDENTITY`, `FAKE_CONTENT`, `SUICIDAL`, `INACCURATE_MEMBER_INFORMATION`, `DECEASED`, `SEEN_OFTEN`, `BROKEN_LINKS`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

