---
title: "Update onenoteOperation"
description: "Update the properties of a onenoteOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update onenoteOperation

Namespace: microsoft.graph

Update the properties of a [onenoteOperation](../resources/onenoteoperation.md) object.

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
PATCH /me/joinedGroups/{groupId}/sites/{siteId}/onenote/operations/{onenoteOperationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [onenoteOperation](../resources/onenoteoperation.md) object.

The following table shows the properties that are required when you create the [onenoteOperation](../resources/onenoteoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Inherited from [operation](../resources/operation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|createdDateTime|DateTimeOffset| Inherited from [operation](../resources/operation.md)|
|lastActionDateTime|DateTimeOffset| Inherited from [operation](../resources/operation.md)|
|resourceLocation|String||
|resourceId|String||
|error|[onenoteOperationError](../resources/onenoteoperationerror.md)||
|percentComplete|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [onenoteOperation](../resources/onenoteoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_onenoteoperation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/sites/{siteId}/onenote/operations/{onenoteOperationId}
Content-type: application/json
Content-length: 419

{
  "@odata.type": "#microsoft.graph.onenoteOperation",
  "status": "String",
  "lastActionDateTime": "2016-12-31T23:59:45.6080321+03:00",
  "resourceLocation": "Resource Location value",
  "resourceId": "Resource Id value",
  "error": {
    "@odata.type": "microsoft.graph.onenoteOperationError",
    "code": "Code value",
    "message": "Message value"
  },
  "percentComplete": "Percent Complete value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 527

{
  "@odata.type": "#microsoft.graph.onenoteOperation",
  "id": "e19b3021-3021-e19b-2130-9be121309be1",
  "status": "String",
  "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
  "lastActionDateTime": "2016-12-31T23:59:45.6080321+03:00",
  "resourceLocation": "Resource Location value",
  "resourceId": "Resource Id value",
  "error": {
    "@odata.type": "microsoft.graph.onenoteOperationError",
    "code": "Code value",
    "message": "Message value"
  },
  "percentComplete": "Percent Complete value"
}
```

