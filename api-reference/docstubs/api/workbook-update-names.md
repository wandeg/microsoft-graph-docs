---
title: "Update names"
description: "Update the properties of a names object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update names

Namespace: microsoft.graph

Update the properties of a names object.

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
PATCH /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [workbookNamedItem](../resources/workbooknameditem.md) object.

The following table shows the properties that are required when you create the [workbookNamedItem](../resources/workbooknameditem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|comment|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|scope|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|value|[Json](../resources/json.md)|**TODO: Add Description**|
|visible|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_names"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names
Content-Type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.workbookNamedItem",
  "comment": "Comment value",
  "name": "Name value",
  "scope": "Scope value",
  "type": "Type value",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  },
  "visible": true
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
  "@odata.type": "#microsoft.graph.workbookNamedItem",
  "id": "873999a7-99a7-8739-a799-3987a7993987",
  "comment": "Comment value",
  "name": "Name value",
  "scope": "Scope value",
  "type": "Type value",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  },
  "visible": true
}
```

