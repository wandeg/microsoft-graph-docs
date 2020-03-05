---
title: "move"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# move

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
POST ** Entity URI for microsoft.graph.mailSearchFolder not found/move
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|DestinationId|String||



## Response
If successful, this action returns a `200 OK` response code and a [mailFolder](../resources/mailfolder.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "mailsearchfolder_move"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.mailSearchFolder not found/move

Content-type: application/json
Content-length: 47

{
  "DestinationId": "Destination Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailfolder"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "value": {
    "@odata.type": "#microsoft.graph.mailFolder",
    "id": "d94961bc-61bc-d949-bc61-49d9bc6149d9",
    "displayName": "Display Name value",
    "parentFolderId": "Parent Folder Id value",
    "childFolderCount": 0,
    "unreadItemCount": 15,
    "totalItemCount": 14
  }
}
```

