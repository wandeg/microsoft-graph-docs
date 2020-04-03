---
title: "getByIds"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getByIds

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
POST /directoryObjects/getByIds
POST /directory/deletedItems/getByIds
POST /groups/{groupsId}/acceptedSenders/getByIds
POST /groups/{groupsId}/rejectedSenders/getByIds
POST /me/joinedTeams/{groupId}/acceptedSenders/getByIds
POST /me/joinedTeams/{groupId}/rejectedSenders/getByIds
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
|ids|String collection||
|types|String collection||



## Response
If successful, this action returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "directoryobject_getbyids"
}
-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds

Content-type: application/json
Content-length: 77

{
  "ids": [
    "Ids value"
  ],
  "types": [
    "Types value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directoryobject)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directoryObject",
      "id": "1f6c5d4c-5d4c-1f6c-4c5d-6c1f4c5d6c1f",
      "deletedDateTime": "2016-12-31T23:59:29.9270269+00:00"
    }
  ]
}
```

