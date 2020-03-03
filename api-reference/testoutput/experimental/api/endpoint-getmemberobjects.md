---
title: "getMemberObjects"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getMemberObjects



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
POST /groups/{groupsId}/endpoints/{endpointId}/getMemberObjects
POST /me/joinedGroups/{groupId}/endpoints/{endpointId}/getMemberObjects
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
|securityEnabledOnly|Boolean||



## Response
If successful, this action returns a `200 OK` response code and a String collection in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "endpoint_getmemberobjects"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/groups/{groupsId}/endpoints/{endpointId}/getMemberObjects

Content-type: application/json
Content-length: 35

{
  "securityEnabledOnly": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(edm.string)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 55

{
  "value": [
    "Get Member Objects value"
  ]
}
```

