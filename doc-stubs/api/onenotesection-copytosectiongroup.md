---
title: "onenoteSection: copyToSectionGroup"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# copyToSectionGroup

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /me/onenote/sections/{onenoteSectionId}/copyToSectionGroup
POST /users/{usersId}/onenote/sections/{onenoteSectionId}/copyToSectionGroup
POST /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/copyToSectionGroup
POST /users/{usersId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/copyToSectionGroup
POST /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}/parentSection/copyToSectionGroup
POST /me/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/sections/{onenoteSectionId}/copyToSectionGroup
POST /users/{usersId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}/parentSection/copyToSectionGroup
POST /users/{usersId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/sections/{onenoteSectionId}/copyToSectionGroup
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|groupId|String|**TODO: Add Description**|
|renameAs|String|**TODO: Add Description**|
|siteCollectionId|String|**TODO: Add Description**|
|siteId|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [onenoteOperation](../resources/onenoteoperation.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "onenotesection_copytosectiongroup"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/onenote/sections/{onenoteSectionId}/copyToSectionGroup

Content-Type: application/json
Content-length: 127

{
  "id": "String",
  "groupId": "String",
  "renameAs": "String",
  "siteCollectionId": "String",
  "siteId": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteoperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.onenoteOperation",
    "id": "String (identifier)",
    "status": "String",
    "createdDateTime": "String (timestamp)",
    "lastActionDateTime": "String (timestamp)",
    "resourceLocation": "String",
    "resourceId": "String",
    "error": {
      "@odata.type": "microsoft.graph.onenoteOperationError"
    },
    "percentComplete": "String"
  }
}
```

