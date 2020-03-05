---
title: "List windows10CustomConfigurations"
description: "List properties and relationships of the windows10CustomConfiguration objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List windows10CustomConfigurations

Namespace: microsoft.graph

List properties and relationships of the [windows10CustomConfiguration](../resources/windows10customconfiguration.md) objects.

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
GET ** Collection URI for microsoft.graph.windows10CustomConfiguration not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [windows10CustomConfiguration](../resources/windows10customconfiguration.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windows10customconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.windows10CustomConfiguration not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windows10customconfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
      "id": "aaec705b-705b-aaec-5b70-ecaa5b70ecaa",
      "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```

