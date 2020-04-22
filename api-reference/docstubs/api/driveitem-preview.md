---
title: "driveItem: preview"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# preview

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
POST /drive/root/preview
POST /drives/{drivesId}/root/preview
POST /shares/{sharesId}/root/preview
POST /workbooks/{workbooksId}/preview
POST /drive/items/{driveItemId}/preview
POST /shares/{sharesId}/driveItem/preview
POST /drive/bundles/{driveItemId}/preview
POST /drive/special/{driveItemId}/preview
POST /drive/following/{driveItemId}/preview
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
|viewer|String|**TODO: Add Description**|
|chromeless|Boolean|**TODO: Add Description**|
|allowEdit|Boolean|**TODO: Add Description**|
|page|String|**TODO: Add Description**|
|zoom|Double|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [itemPreviewInfo](../resources/itempreviewinfo.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "driveitem_preview"
}
-->
``` http
POST https://graph.microsoft.com/beta/drive/root/preview

Content-Type: application/json
Content-length: 123

{
  "viewer": "Viewer value",
  "chromeless": true,
  "allowEdit": true,
  "page": "Page value",
  "zoom": "Double"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itempreviewinfo"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "microsoft.graph.itemPreviewInfo"
  }
}
```

