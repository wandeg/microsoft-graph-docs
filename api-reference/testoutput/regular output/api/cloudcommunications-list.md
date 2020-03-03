---
title: "List cloudCommunicationses"
description: "List properties and relationships of the cloudCommunications objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List cloudCommunicationses

List properties and relationships of the [cloudCommunications](../resources/cloudcommunications.md) objects.

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
GET ** Collection URI for microsoft.graph.cloudCommunications not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [cloudCommunications](../resources/cloudcommunications.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_cloudcommunications"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.cloudCommunications not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.cloudcommunications)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudCommunications",
      "id": "a0b64534-4534-a0b6-3445-b6a03445b6a0"
    }
  ]
}
```

