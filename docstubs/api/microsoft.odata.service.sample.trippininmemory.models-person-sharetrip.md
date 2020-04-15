---
title: "person: shareTrip"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# shareTrip

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



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
POST /me/shareTrip
POST /people/{peopleId}/shareTrip
POST /newComePeople/{newComePeopleId}/shareTrip
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|userName|String||
|tripId|Int32||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "person_sharetrip"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/shareTrip

Content-type: application/json
Content-length: 53

{
  "userName": "User Name value",
  "tripId": 6
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

