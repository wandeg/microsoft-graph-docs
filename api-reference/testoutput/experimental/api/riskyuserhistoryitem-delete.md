---
title: "Delete riskyUserHistoryItem"
description: "Deletes a riskyUserHistoryItem."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete riskyUserHistoryItem

Namespace: microsoft.graph

Deletes a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md).

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
DELETE /riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}
DELETE /riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}/history/{riskyUserHistoryItemId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "delete_riskyuserhistoryitem"
}
-->
``` http
DELETE https://graph.microsoft.com/localtest/riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

