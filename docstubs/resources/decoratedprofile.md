---
title: "DecoratedProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# DecoratedProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List DecoratedProfiles](../api/decoratedprofile-list.md)|[DecoratedProfile](../resources/decoratedprofile.md) collection|List properties and relationships of the [DecoratedProfile](../resources/decoratedprofile.md) objects.|
|[Get DecoratedProfile](../api/decoratedprofile-get.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Read properties and relationships of the [DecoratedProfile](../resources/decoratedprofile.md) object.|
|[Create DecoratedProfile](../api/decoratedprofile-post-decoratedprofiles.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Create a new [DecoratedProfile](../resources/decoratedprofile.md) object.|
|[Delete DecoratedProfile](../api/decoratedprofile-delete.md)|None|Deletes a [DecoratedProfile](../resources/decoratedprofile.md).|
|[Update DecoratedProfile](../api/decoratedprofile-update.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Update the properties of a [DecoratedProfile](../resources/decoratedprofile.md) object.|
|[viewees](../api/decoratedprofile-viewees.md)|[DecoratedProfile](../resources/decoratedprofile.md) collection||
|[batchGet](../api/decoratedprofile-batchget.md)|[DecoratedProfileBatchGetResult](../resources/decoratedprofilebatchgetresult.md)||
|[List profiles](../api/decoratedprofilesearchresult-list-profiles.md)|[DecoratedProfile](../resources/decoratedprofile.md) collection|Get the DecoratedProfiles from the profiles navigation property.|
|[Add profiles](../api/decoratedprofilesearchresult-post-profiles.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Add profiles by posting to the profiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bornOn|[Date](../resources/date.md)||
|connected|Boolean||
|connection|[Connection](../resources/connection.md)||
|connectionDegree|Enumeration| Possible values are: `OUT_OF_NETWORK`, `SELF`, `DISTANCE_1`, `DISTANCE_2`, `DISTANCE_3`.|
|emails|String collection||
|firstName|String||
|headline|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|ims|[IM](../resources/im.md) collection||
|industryName|String||
|invitationSentFromViewer|Boolean||
|lastName|String||
|locale|[Locale](../resources/locale.md)||
|location|String||
|pendingInvitationSentFromViewee|[liInvitation](../resources/liinvitation.md)||
|phoneNumbers|[PhoneNumber](../resources/phonenumber.md) collection||
|picture|String||
|profileHighlights|[DecoratedProfileProfileHighlights](../resources/decoratedprofileprofilehighlights.md) collection||
|profileUrl|String||
|recentEducations|[Education](../resources/education.md) collection||
|recentPositions|[Position](../resources/position.md) collection||
|salesNavigatorInfo|[SalesNavigatorInfo](../resources/salesnavigatorinfo.md)||
|simpleProfileHighlights|[SimpleProfileHighlight](../resources/simpleprofilehighlight.md) collection||
|skills|String collection||
|summary|String||
|totalEducationCount|Int32||
|totalPositionCount|Int32||
|viewerCanConnectViewee|Boolean||
|viewerCanFollowViewee|Boolean||
|websites|[liWebsite](../resources/liwebsite.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "totalPositionCount": 1024,
  "recentEducations": [
    {
      "@odata.type": "microsoft.graph.Education"
    }
  ],
  "totalEducationCount": 1024,
  "skills": [
    "String"
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
  "connected": true,
  "connectionDegree": "String",
  "invitationSentFromViewer": true,
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
  "viewerCanConnectViewee": true,
  "viewerCanFollowViewee": true,
  "salesNavigatorInfo": {
    "@odata.type": "microsoft.graph.SalesNavigatorInfo"
  }
}
```

