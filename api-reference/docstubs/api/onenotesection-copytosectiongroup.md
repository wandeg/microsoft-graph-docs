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
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/sections/{onenoteSectionId}/copyToSectionGroup
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/copyToSectionGroup
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}/parentSection/copyToSectionGroup
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/sections/{onenoteSectionId}/copyToSectionGroup
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/sections/{onenoteSectionId}/copyToSectionGroup

Content-Type: application/json
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
    "id": "2291d582-d582-2291-82d5-912282d59122",
    "status": "String",
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
    "lastActionDateTime": "2016-12-31T23:57:13.8078619+03:00",
    "resourceLocation": "Resource Location value",
    "resourceId": "Resource Id value",
    "error": {
      "@odata.type": "microsoft.graph.onenoteOperationError"
    },
    "percentComplete": "Percent Complete value"
  }
}
```

