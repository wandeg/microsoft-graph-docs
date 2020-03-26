---
title: "getUserOwnedObjects"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getUserOwnedObjects

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
POST /directoryObjects/getUserOwnedObjects
POST /directory/deletedItems/getUserOwnedObjects
POST /groups/{groupsId}/acceptedSenders/getUserOwnedObjects
POST /groups/{groupsId}/rejectedSenders/getUserOwnedObjects
POST /me/joinedGroups/{groupId}/acceptedSenders/getUserOwnedObjects
POST /me/joinedGroups/{groupId}/rejectedSenders/getUserOwnedObjects
POST /directory/featureRolloutPolicies/{featureRolloutPolicyId}/appliesTo/getUserOwnedObjects
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
|userId|String||
|type|String||



## Response
If successful, this action returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "directoryobject_getuserownedobjects"
}
-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/getUserOwnedObjects

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
    "id": "4c87ac4e-ac4e-4c87-4eac-874c4eac874c",
    "deletedDateTime": "2016-12-31T23:58:50.3020202+00:00"
  }
}
```

