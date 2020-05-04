---
title: "driveItem: validatePermission"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# validatePermission

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
POST /drive/root/validatePermission
POST /drives/{drivesId}/root/validatePermission
POST /shares/{sharesId}/root/validatePermission
POST /workbooks/{workbooksId}/validatePermission
POST /drive/items/{driveItemId}/validatePermission
POST /shares/{sharesId}/driveItem/validatePermission
POST /drive/bundles/{driveItemId}/validatePermission
POST /drive/special/{driveItemId}/validatePermission
POST /drive/following/{driveItemId}/validatePermission
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
|challengeToken|String|**TODO: Add Description**|
|password|String|**TODO: Add Description**|



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "driveitem_validatepermission"
}
-->
``` http
POST https://graph.microsoft.com/beta/drive/root/validatePermission

Content-Type: application/json
Content-length: 82

{
  "challengeToken": "Challenge Token value",
  "password": "Password value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

