---
title: "List settings"
description: "Get the directorySettings from the settings navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List settings

Namespace: microsoft.graph

Get the directorySettings from the settings navigation property.

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
GET /groups/{groupsId}/settings
GET /me/joinedGroups/{groupId}/settings
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [directorySetting](../resources/directorysetting.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groups/{groupsId}/settings
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directorysetting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directorySetting",
      "id": "95cf0a68-0a68-95cf-680a-cf95680acf95",
      "displayName": "Display Name value",
      "templateId": "Template Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.settingValue",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

