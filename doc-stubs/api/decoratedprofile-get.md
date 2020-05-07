---
title: "Get DecoratedProfile"
description: "Read the properties and relationships of a DecoratedProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get DecoratedProfile

Namespace: microsoft.graph

Read the properties and relationships of a [DecoratedProfile](../resources/decoratedprofile.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /decoratedProfiles/{decoratedProfilesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [DecoratedProfile](../resources/decoratedprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_decoratedprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/decoratedProfiles/{decoratedProfilesId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.DecoratedProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.DecoratedProfile",
    "id": "16be6d7e-6d7e-16be-7e6d-be167e6dbe16",
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

