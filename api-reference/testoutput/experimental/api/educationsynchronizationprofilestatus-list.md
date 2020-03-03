---
title: "List educationSynchronizationProfileStatuses"
description: "List properties and relationships of the educationSynchronizationProfileStatus objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List educationSynchronizationProfileStatuses

Namespace: microsoft.graph

List properties and relationships of the [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) objects.

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
GET ** Collection URI for microsoft.graph.educationSynchronizationProfileStatus not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationsynchronizationprofilestatus"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.educationSynchronizationProfileStatus not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationsynchronizationprofilestatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
      "id": "982895ee-95ee-9828-ee95-2898ee952898",
      "status": "String",
      "lastSynchronizationDateTime": "2016-12-31T23:59:53.6736225+03:00"
    }
  ]
}
```

