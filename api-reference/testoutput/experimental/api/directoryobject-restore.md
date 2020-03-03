---
title: "restore"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# restore



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
POST /directoryObjects/{directoryObjectsId}/restore
POST /directory/deletedItems/{directoryObjectId}/restore
POST /groups/{groupsId}/acceptedSenders/{directoryObjectId}/restore
POST /groups/{groupsId}/rejectedSenders/{directoryObjectId}/restore
POST /me/joinedGroups/{groupId}/acceptedSenders/{directoryObjectId}/restore
POST /me/joinedGroups/{groupId}/rejectedSenders/{directoryObjectId}/restore
POST /directory/featureRolloutPolicies/{featureRolloutPolicyId}/appliesTo/{directoryObjectId}/restore
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [directoryObject](../resources/directoryObject.md) in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "directoryobject_restore"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/directoryObjects/{directoryObjectsId}/restore
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryobject"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 190

{
  "value": {
    "@odata.type": "#microsoft.graph.directoryObject",
    "id": "98b7e341-e341-98b7-41e3-b79841e3b798",
    "deletedDateTime": "2017-01-01T00:00:34.0507931+03:00"
  }
}
```

