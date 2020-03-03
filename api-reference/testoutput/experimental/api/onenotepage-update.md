---
title: "Update onenotePage"
description: "Update the properties of a onenotePage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update onenotePage

Namespace: microsoft.graph

Update the properties of a [onenotePage](../resources/onenotepage.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/joinedGroups/{groupId}/sites/{siteId}/onenote/pages/{onenotePageId}
PATCH /me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [onenotePage](../resources/onenotepage.md) object.

The following table shows the properties that are required when you create the [onenotePage](../resources/onenotepage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|title|String||
|createdByAppId|String||
|links|[pageLinks](../resources/pagelinks.md)||
|contentUrl|String||
|content|Stream||
|lastModifiedDateTime|DateTimeOffset||
|level|Int32||
|order|Int32||
|userTags|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [onenotePage](../resources/onenotepage.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_onenotepage"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/sites/{siteId}/onenote/pages/{onenotePageId}
Content-type: application/json
Content-length: 575

{
  "@odata.type": "#microsoft.graph.onenotePage",
  "self": "Self value",
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
  "level": 5,
  "order": 5,
  "userTags": [
    "User Tags value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 746

{
  "@odata.type": "#microsoft.graph.onenotePage",
  "id": "c1ca2dc3-2dc3-c1ca-c32d-cac1c32dcac1",
  "self": "Self value",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
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
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "level": 5,
  "order": 5,
  "userTags": [
    "User Tags value"
  ]
}
```

