---
title: "Get directoryObject"
description: "Read properties and relationships of a directoryObject object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get directoryObject

Namespace: microsoft.graph

Read properties and relationships of a [directoryObject](../resources/directoryobject.md) object.

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
GET /directoryObjects/{directoryObjectsId}
GET /directory/deletedItems/{directoryObjectId}
GET /groups/{groupsId}/acceptedSenders/{directoryObjectId}
GET /groups/{groupsId}/rejectedSenders/{directoryObjectId}
GET /me/joinedGroups/{groupId}/acceptedSenders/{directoryObjectId}
GET /me/joinedGroups/{groupId}/rejectedSenders/{directoryObjectId}
GET /directory/featureRolloutPolicies/{featureRolloutPolicyId}/appliesTo/{directoryObjectId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}
-->
``` http
GET https://graph.microsoft.com/beta/directoryObjects/{directoryObjectsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.directoryObject",
    "id": "2c50d09a-d09a-2c50-9ad0-502c9ad0502c",
    "deletedDateTime": "2017-01-01T00:03:10.8575862+03:00"
  }
}
```

