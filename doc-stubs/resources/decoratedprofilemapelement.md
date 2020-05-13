---
title: "DecoratedProfileMapElement resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# DecoratedProfileMapElement resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|key|String|**TODO: Add Description**|
|value|[DecoratedProfile](../resources/decoratedprofile.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.DecoratedProfileMapElement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.DecoratedProfileMapElement",
  "key": "String",
  "value": {
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
    "viewerCanConnectViewee": "Boolean",
    "viewerCanFollowViewee": "Boolean",
    "salesNavigatorInfo": {
      "@odata.type": "microsoft.graph.SalesNavigatorInfo"
    }
  }
}
```

