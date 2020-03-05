---
title: "Get androidWorkProfileCustomConfiguration"
description: "Read properties and relationships of the androidWorkProfileCustomConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get androidWorkProfileCustomConfiguration

Namespace: microsoft.graph

Read properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/androidworkprofilecustomconfiguration.md) object.

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
GET ** Entity URI for microsoft.graph.androidWorkProfileCustomConfiguration not found
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
If successful, this method returns a `200 OK` response code and [androidWorkProfileCustomConfiguration](../resources/androidworkprofilecustomconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_androidworkprofilecustomconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.androidWorkProfileCustomConfiguration not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidWorkProfileCustomConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
    "id": "567c17d8-17d8-567c-d817-7c56d8177c56",
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

