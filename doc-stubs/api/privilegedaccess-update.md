---
title: "Update privilegedAccess"
description: "Update the properties of a privilegedAccess object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update privilegedAccess

Namespace: microsoft.graph

Update the properties of a [privilegedAccess](../resources/privilegedaccess.md) object.

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
PATCH /privilegedAccess/{privilegedAccessId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [privilegedAccess](../resources/privilegedaccess.md) object.

The following table shows the properties that are required when you create the [privilegedAccess](../resources/privilegedaccess.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [privilegedAccess](../resources/privilegedaccess.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_privilegedaccess"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedAccess/{privilegedAccessId}
Content-Type: application/json
Content-length: 86

{
  "@odata.type": "#microsoft.graph.privilegedAccess",
  "displayName": "String"
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
  "@odata.type": "#microsoft.graph.privilegedAccess",
  "id": "b7543cf9-3cf9-b754-f93c-54b7f93c54b7",
  "displayName": "String"
}
```

