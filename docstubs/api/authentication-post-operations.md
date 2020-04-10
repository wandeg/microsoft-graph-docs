---
title: "Add operations"
description: "Add operations by posting to the operations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add operations

Namespace: microsoft.graph

Add operations by posting to the operations collection.

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
POST /me/authentication/operations/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [longRunningOperation](../resources/longrunningoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_longrunningoperation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/authentication/operations
Content-type: application/json
Content-length: 239

{
  "@odata.type": "#microsoft.graph.longRunningOperation",
  "lastActionDateTime": "2016-12-31T23:58:44.1540706+00:00",
  "status": "String",
  "statusDetail": "Status Detail value",
  "resourceLocation": "Resource Location value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.longrunningoperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 347

{
  "@odata.type": "#microsoft.graph.longRunningOperation",
  "id": "dcb776c6-76c6-dcb7-c676-b7dcc676b7dc",
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
  "lastActionDateTime": "2016-12-31T23:58:44.1540706+00:00",
  "status": "String",
  "statusDetail": "Status Detail value",
  "resourceLocation": "Resource Location value"
}
```

