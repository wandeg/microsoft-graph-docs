---
title: "Get onenotePage"
description: "Read properties and relationships of an onenotePage object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get onenotePage

Namespace: microsoft.graph

Read properties and relationships of an [onenotePage](../resources/onenotepage.md) object.

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
GET /invitations/{invitationsId}/invitedUser/onenote/pages/{onenotePageId}
GET /invitations/{invitationsId}/invitedUser/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [onenotePage](../resources/onenotepage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_onenotepage"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/onenote/pages/{onenotePageId}
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
{
  "value": {
    "@odata.type": "#microsoft.graph.onenotePage",
    "id": "561dbd6e-bd6e-561d-6ebd-1d566ebd1d56",
    "self": "Self value",
    "createdDateTime": "2017-01-01T00:01:28.5453509+00:00",
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
    "lastModifiedDateTime": "2017-01-01T00:01:26.0388723+00:00",
    "level": 5,
    "order": 5,
    "userTags": [
      "User Tags value"
    ]
  }
}
```

