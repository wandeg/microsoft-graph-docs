---
title: "List userConfigurations"
description: "List properties and relationships of the userConfiguration objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userConfigurations

Namespace: microsoft.graph

List properties and relationships of the [userConfiguration](../resources/userconfiguration.md) objects.

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
GET /me/mailFolders/{mailFolderId}/userConfigurations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [userConfiguration](../resources/userconfiguration.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/mailFolders/{mailFolderId}/userConfigurations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.userconfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 190

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userConfiguration",
      "id": "0e1870cb-70cb-0e18-cb70-180ecb70180e",
      "binaryData": "YmluYXJ5RGF0YQ=="
    }
  ]
}
```

