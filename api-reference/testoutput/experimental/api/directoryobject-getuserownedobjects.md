---
title: "getUserOwnedObjects"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getUserOwnedObjects



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
POST /directoryObjects/getUserOwnedObjects
POST /directory/deletedItems/getUserOwnedObjects
POST /groups/{groupsId}/acceptedSenders/getUserOwnedObjects
POST /groups/{groupsId}/rejectedSenders/getUserOwnedObjects
POST /me/joinedGroups/{groupId}/acceptedSenders/getUserOwnedObjects
POST /me/joinedGroups/{groupId}/rejectedSenders/getUserOwnedObjects
POST /directory/featureRolloutPolicies/{featureRolloutPolicyId}/appliesTo/getUserOwnedObjects
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
|userId|String||
|type|String||



## Response
If successful, this action returns a `200 OK` response code and a [directoryObject](../resources/directoryObject.md) in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "directoryobject_getuserownedobjects"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/directoryObjects/getUserOwnedObjects

Content-type: application/json
Content-length: 58

{
  "userId": "User Id value",
  "type": "Type value"
}
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

