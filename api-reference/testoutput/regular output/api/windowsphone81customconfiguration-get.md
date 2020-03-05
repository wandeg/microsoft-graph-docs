---
title: "Get windowsPhone81CustomConfiguration"
description: "Read properties and relationships of the windowsPhone81CustomConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get windowsPhone81CustomConfiguration

Namespace: microsoft.graph

Read properties and relationships of the [windowsPhone81CustomConfiguration](../resources/windowsphone81customconfiguration.md) object.

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
GET ** Entity URI for microsoft.graph.windowsPhone81CustomConfiguration not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [windowsPhone81CustomConfiguration](../resources/windowsphone81customconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsphone81customconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.windowsPhone81CustomConfiguration not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsPhone81CustomConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
    "id": "0d65226a-226a-0d65-6a22-650d6a22650d",
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
}
```

