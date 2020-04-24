---
title: "Get onenotePage"
description: "Read the properties and relationships of an onenotePage object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get onenotePage

Namespace: microsoft.graph

Read the properties and relationships of an [onenotePage](../resources/onenotepage.md) object.

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
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/pages/{onenotePageId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}
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
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/pages/{onenotePageId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
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
    "id": "5be483e3-83e3-5be4-e383-e45be383e45b",
    "self": "Self value",
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
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
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
    "level": 5,
    "order": 5,
    "userTags": [
      "User Tags value"
    ]
  }
}
```

