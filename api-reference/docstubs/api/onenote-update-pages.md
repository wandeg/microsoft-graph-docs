---
title: "Update pages"
description: "Update the properties of a pages object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update pages

Namespace: microsoft.graph

Update the properties of a pages object.

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
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/pages
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [onenotePage](../resources/onenotepage.md) object.

The following table shows the properties that are required when you create the [onenotePage](../resources/onenotepage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|self|String|**TODO: Add Description** Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|title|String|**TODO: Add Description**|
|createdByAppId|String|**TODO: Add Description**|
|links|[pageLinks](../resources/pagelinks.md)|**TODO: Add Description**|
|contentUrl|String|**TODO: Add Description**|
|content|Stream|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|level|Int32|**TODO: Add Description**|
|order|Int32|**TODO: Add Description**|
|userTags|String collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [onenotePage](../resources/onenotepage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_pages"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/pages
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
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
```

