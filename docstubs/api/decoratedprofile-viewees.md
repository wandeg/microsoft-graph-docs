---
title: "viewees"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# viewees

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /decoratedProfiles/viewees
GET /decoratedProfileSearchResults/{decoratedProfileSearchResultsId}/profiles/viewees
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|viewees|String collection||



## Response
If successful, this function returns a `200 OK` response code and a [DecoratedProfile](../resources/decoratedprofile.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "decoratedprofile_viewees"
}
-->
``` http
GET https://graph.microsoft.com/beta/decoratedProfiles/viewees(viewees=[
  "Viewees value"
])
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.decoratedprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2093

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.DecoratedProfile",
      "id": "da23c855-c855-da23-55c8-23da55c823da",
      "profileUrl": "https://example.com/profileUrl/",
      "firstName": "First Name value",
      "lastName": "Last Name value",
      "headline": "Headline value",
      "industryName": "Industry Name value",
      "summary": "Summary value",
      "location": "Location value",
      "picture": "Picture value",
      "recentPositions": [
        {
          "@odata.type": "microsoft.graph.Position"
        }
      ],
      "totalPositionCount": 2,
      "recentEducations": [
        {
          "@odata.type": "microsoft.graph.Education"
        }
      ],
      "totalEducationCount": 3,
      "skills": [
        "Skills value"
      ],
      "emails": [
        "Emails value"
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
  ]
}
```

