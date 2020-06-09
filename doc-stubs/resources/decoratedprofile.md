---
title: "DecoratedProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# DecoratedProfile resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List DecoratedProfiles](../api/decoratedprofile-list.md)|[DecoratedProfile](../resources/decoratedprofile.md) collection|Get a list of the [DecoratedProfile](../resources/decoratedprofile.md) objects and their properties.|
|[Create DecoratedProfile](../api/decoratedprofile-post-decoratedprofiles.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Create a new [DecoratedProfile](../resources/decoratedprofile.md) object.|
|[Get DecoratedProfile](../api/decoratedprofile-get.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Read the properties and relationships of a [DecoratedProfile](../resources/decoratedprofile.md) object.|
|[Update DecoratedProfile](../api/decoratedprofile-update.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Update the properties of a [DecoratedProfile](../resources/decoratedprofile.md) object.|
|[Delete DecoratedProfile](../api/decoratedprofile-delete.md)|None|Deletes a [DecoratedProfile](../resources/decoratedprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bornOn|[Date](../resources/date.md)|**TODO: Add Description**|
|connected|Boolean|**TODO: Add Description**|
|connection|[Connection](../resources/connection.md)|**TODO: Add Description**|
|connectionDegree|ConnectionDegree|**TODO: Add Description**. Possible values are: `OUT_OF_NETWORK`, `SELF`, `DISTANCE_1`, `DISTANCE_2`, `DISTANCE_3`.|
|emails|String collection|**TODO: Add Description**|
|endorsedSkills|[SkillEndorsement](../resources/skillendorsement.md) collection|**TODO: Add Description**|
|firstName|String|**TODO: Add Description**|
|headline|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|ims|[IM](../resources/im.md) collection|**TODO: Add Description**|
|industryName|String|**TODO: Add Description**|
|invitationSentFromViewer|Boolean|**TODO: Add Description**|
|lastName|String|**TODO: Add Description**|
|locale|[Locale](../resources/locale.md)|**TODO: Add Description**|
|location|String|**TODO: Add Description**|
|newsMentions|[NewsMention](../resources/newsmention.md) collection|**TODO: Add Description**|
|pendingInvitationSentFromViewee|[liInvitation](../resources/liinvitation.md)|**TODO: Add Description**|
|phoneNumbers|[PhoneNumber](../resources/phonenumber.md) collection|**TODO: Add Description**|
|picture|String|**TODO: Add Description**|
|profileHighlights|[DecoratedProfileProfileHighlights](../resources/decoratedprofileprofilehighlights.md) collection|**TODO: Add Description**|
|profileUrl|String|**TODO: Add Description**|
|recentEducations|[Education](../resources/education.md) collection|**TODO: Add Description**|
|recentPositions|[Position](../resources/position.md) collection|**TODO: Add Description**|
|salesNavigatorInfo|[SalesNavigatorInfo](../resources/salesnavigatorinfo.md)|**TODO: Add Description**|
|simpleProfileHighlights|[SimpleProfileHighlight](../resources/simpleprofilehighlight.md) collection|**TODO: Add Description**|
|skills|String collection|**TODO: Add Description**|
|summary|String|**TODO: Add Description**|
|totalEducationCount|Int32|**TODO: Add Description**|
|totalPositionCount|Int32|**TODO: Add Description**|
|userGeneratedContents|[UserGeneratedContent](../resources/usergeneratedcontent.md) collection|**TODO: Add Description**|
|viewerCanConnectViewee|Boolean|**TODO: Add Description**|
|viewerCanFollowViewee|Boolean|**TODO: Add Description**|
|websites|[liWebsite](../resources/liwebsite.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.DecoratedProfile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
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
```

