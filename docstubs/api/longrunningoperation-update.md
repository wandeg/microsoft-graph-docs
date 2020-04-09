---
title: "Update longRunningOperation"
description: "Update the properties of a longRunningOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update longRunningOperation

Namespace: microsoft.graph

Update the properties of a [longRunningOperation](../resources/longrunningoperation.md) object.

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
PATCH /me/authentication/operations/{longRunningOperationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [longRunningOperation](../resources/longrunningoperation.md) object.

The following table shows the properties that are required when you create the [longRunningOperation](../resources/longrunningoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset||
|lastActionDateTime|DateTimeOffset||
|status|Enumeration| Possible values are: `notstarted`, `running`, `succeeded`, `failed`.|
|statusDetail|String||
|resourceLocation|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [longRunningOperation](../resources/longrunningoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_longrunningoperation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/authentication/operations/{longRunningOperationId}
Content-type: application/json
Content-length: 239

{
  "@odata.type": "#microsoft.graph.longRunningOperation",
  "lastActionDateTime": "2017-01-01T00:02:09.4916918+03:00",
  "status": "String",
  "statusDetail": "Status Detail value",
  "resourceLocation": "Resource Location value"
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
Content-Length: 347

{
  "@odata.type": "#microsoft.graph.longRunningOperation",
  "id": "70cd0ba0-0ba0-70cd-a00b-cd70a00bcd70",
  "createdDateTime": "2017-01-01T00:00:01.0610721+03:00",
  "lastActionDateTime": "2017-01-01T00:02:09.4916918+03:00",
  "status": "String",
  "statusDetail": "Status Detail value",
  "resourceLocation": "Resource Location value"
}
```

