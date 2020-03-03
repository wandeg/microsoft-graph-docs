---
title: "List notebooks"
description: "List properties and relationships of the notebook objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List notebooks

Namespace: microsoft.graph

List properties and relationships of the [notebook](../resources/notebook.md) objects.

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
GET /me/onenote/notebooks
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [notebook](../resources/notebook.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/onenote/notebooks
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.notebook)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1330

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.notebook",
      "id": "b4d3cd84-cd84-b4d3-84cd-d3b484cdd3b4",
      "self": "Self value",
      "createdDateTime": "2017-01-01T00:02:24.618735+03:00",
      "displayName": "Display Name value",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet",
        "application": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value"
        },
        "device": {
          "@odata.type": "microsoft.graph.identity"
        },
        "user": {
          "@odata.type": "microsoft.graph.identity"
        }
      },
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2017-01-01T00:00:08.5199759+03:00",
      "isDefault": true,
      "userRole": "String",
      "isShared": true,
      "sectionsUrl": "https://example.com/sectionsUrl/",
      "sectionGroupsUrl": "https://example.com/sectionGroupsUrl/",
      "links": {
        "@odata.type": "microsoft.graph.notebookLinks",
        "oneNoteClientUrl": {
          "@odata.type": "microsoft.graph.externalLink",
          "href": "Href value"
        },
        "oneNoteWebUrl": {
          "@odata.type": "microsoft.graph.externalLink"
        }
      }
    }
  ]
}
```

