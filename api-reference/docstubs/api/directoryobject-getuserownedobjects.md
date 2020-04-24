---
title: "directoryObject: getUserOwnedObjects"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getUserOwnedObjects

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /directoryObjects/getUserOwnedObjects
POST /directory/deletedItems/getUserOwnedObjects
POST /groups/{groupsId}/acceptedSenders/getUserOwnedObjects
POST /groups/{groupsId}/rejectedSenders/getUserOwnedObjects
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|userId|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "directoryobject_getuserownedobjects"
}
-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/getUserOwnedObjects

Content-Type: application/json
Content-length: 58

{
  "userId": "User Id value",
  "type": "Type value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryobject"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.directoryObject",
    "id": "e6b95329-5329-e6b9-2953-b9e62953b9e6",
    "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00"
  }
}
```

