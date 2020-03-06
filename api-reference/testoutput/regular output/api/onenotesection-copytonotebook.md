---
title: "copyToNotebook"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# copyToNotebook

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
POST /me/onenote/sections/{onenoteSectionId}/copyToNotebook
POST /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/copyToNotebook
POST /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}/parentSection/copyToNotebook
POST /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/sections/{onenoteSectionId}/copyToNotebook
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|id|String||
|groupId|String||
|renameAs|String||
|siteCollectionId|String||
|siteId|String||



## Response
If successful, this action returns a `200 OK` response code and a [onenoteOperation](../resources/onenoteoperation.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "onenotesection_copytonotebook"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/onenote/sections/{onenoteSectionId}/copyToNotebook

Content-type: application/json
Content-length: 171

{
  "id": "Id value",
  "groupId": "Group Id value",
  "renameAs": "Rename As value",
  "siteCollectionId": "Site Collection Id value",
  "siteId": "Site Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteoperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 507

{
  "value": {
    "@odata.type": "#microsoft.graph.onenoteOperation",
    "id": "6e3e20ba-20ba-6e3e-ba20-3e6eba203e6e",
    "status": "String",
    "createdDateTime": "2016-12-31T23:57:43.7581228+03:00",
    "lastActionDateTime": "2017-01-01T00:01:34.678586+03:00",
    "resourceLocation": "Resource Location value",
    "resourceId": "Resource Id value",
    "error": {
      "@odata.type": "microsoft.graph.onenoteOperationError"
    },
    "percentComplete": "Percent Complete value"
  }
}
```

