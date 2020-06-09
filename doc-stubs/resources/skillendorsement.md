---
title: "SkillEndorsement resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# SkillEndorsement resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|endorsementCount|Int32|**TODO: Add Description**|
|endorsers|[DecoratedProfile](../resources/decoratedprofile.md) collection|**TODO: Add Description**|
|skillName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.SkillEndorsement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.SkillEndorsement",
  "skillName": "String",
  "endorsementCount": "Integer",
  "endorsers": [
    {
      "@odata.type": "#microsoft.graph.DecoratedProfile",
      "id": "String (identifier)",
      "profileUrl": "String",
      "firstName": "String",
      "lastName": "String",
      "headline": "String",
      "industryName": "String",
      "summary": "String",
      "location": "String",
      "picture": "String",
      "recentPositions": [
        {
          "@odata.type": "microsoft.graph.Position"
        }
      ],
      "totalPositionCount": "Integer",
      "recentEducations": [
        {
          "@odata.type": "microsoft.graph.Education"
        }
      ],
      "totalEducationCount": "Integer",
      "skills": [
        "String"
      ],
      "endorsedSkills": [
        {
          "@odata.type": "microsoft.graph.SkillEndorsement"
        }
      ],
      "emails": [
        "String"
      ],
      "phoneNumbers": [
        {
          "@odata.type": "microsoft.graph.PhoneNumber"
        }
      ],
      "ims": [
        {
          "@odata.type": "microsoft.graph.IM"
        }
      ],
      "websites": [
        {
          "@odata.type": "microsoft.graph.liWebsite"
        }
      ],
      "bornOn": {
        "@odata.type": "microsoft.graph.Date"
      },
      "locale": {
        "@odata.type": "microsoft.graph.Locale"
      },
      "connection": {
        "@odata.type": "microsoft.graph.Connection"
      },
      "connected": "Boolean",
      "connectionDegree": "String",
      "invitationSentFromViewer": "Boolean",
      "pendingInvitationSentFromViewee": {
        "@odata.type": "microsoft.graph.liInvitation"
      },
      "simpleProfileHighlights": [
        {
          "@odata.type": "microsoft.graph.SimpleProfileHighlight"
        }
      ],
      "profileHighlights": [
        {
          "@odata.type": "microsoft.graph.DecoratedProfileProfileHighlights"
        }
      ],
      "userGeneratedContents": [
        {
          "@odata.type": "microsoft.graph.UserGeneratedContent"
        }
      ],
      "newsMentions": [
        {
          "@odata.type": "microsoft.graph.NewsMention"
        }
      ],
      "viewerCanConnectViewee": "Boolean",
      "viewerCanFollowViewee": "Boolean",
      "salesNavigatorInfo": {
        "@odata.type": "microsoft.graph.SalesNavigatorInfo"
      }
    }
  ]
}
```

