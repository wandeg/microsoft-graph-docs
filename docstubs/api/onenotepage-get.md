---
title: "Get onenotePage"
description: "Read properties and relationships of the onenotePage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get onenotePage

Namespace: microsoft.graph

Read properties and relationships of the [onenotePage](../resources/onenotepage.md) object.

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
GET /me/joinedGroups/{groupId}/sites/{siteId}/onenote/pages/{onenotePageId}
GET /me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [onenotePage](../resources/onenotepage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_onenotepage"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/sites/{siteId}/onenote/pages/{onenotePageId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 814

{
  "value": {
    "@odata.type": "#microsoft.graph.onenotePage",
    "id": "20dd9659-9659-20dd-5996-dd205996dd20",
    "self": "Self value",
    "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
    "title": "Title value",
    "createdByAppId": "Created By App Id value",
    "links": {
      "@odata.type": "microsoft.graph.pageLinks",
      "oneNoteClientUrl": {
        "@odata.type": "microsoft.graph.externalLink",
        "href": "Href value"
      },
      "oneNoteWebUrl": {
        "@odata.type": "microsoft.graph.externalLink"
      }
    },
    "contentUrl": "https://example.com/contentUrl/",
    "content": "Stream",
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
    "level": 5,
    "order": 5,
    "userTags": [
      "User Tags value"
    ]
  }
}
```

