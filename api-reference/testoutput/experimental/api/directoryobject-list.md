---
title: "List directoryObjects"
description: "List properties and relationships of the directoryObject objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List directoryObjects

Namespace: microsoft.graph

List properties and relationships of the [directoryObject](../resources/directoryobject.md) objects.

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
GET /directoryObjects
GET /directory/deletedItems
GET /groups/{groupsId}/acceptedSenders
GET /groups/{groupsId}/rejectedSenders
GET /me/joinedGroups/{groupId}/acceptedSenders
GET /me/joinedGroups/{groupId}/rejectedSenders
GET /directory/featureRolloutPolicies/{featureRolloutPolicyId}/appliesTo
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}
-->
``` http
GET https://graph.microsoft.com/localtest/directoryObjects
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
      "id": "3ee17962-7962-3ee1-6279-e13e6279e13e",
      "deletedDateTime": "2017-01-01T00:00:12.2826741+03:00"
    }
  ]
}
```

