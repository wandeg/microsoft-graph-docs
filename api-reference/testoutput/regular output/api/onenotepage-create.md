---
title: "Create onenotePage"
description: "Create a new onenotePage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create onenotePage

Namespace: microsoft.graph

Create a new [onenotePage](../resources/onenotepage.md) object.

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
POST /me/onenote/pages
POST /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [onenotePage](../resources/onenotepage.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onenotepage_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/onenote/pages
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
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotepage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 745

{
  "@odata.type": "#microsoft.graph.onenotePage",
  "id": "70c2781a-781a-70c2-1a78-c2701a78c270",
  "self": "Self value",
  "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
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
  "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
  "level": 5,
  "order": 5,
  "userTags": [
    "User Tags value"
  ]
}
```

