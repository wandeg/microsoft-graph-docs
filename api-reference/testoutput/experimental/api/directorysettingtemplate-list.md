---
title: "List directorySettingTemplates"
description: "List properties and relationships of the directorySettingTemplate objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List directorySettingTemplates

List properties and relationships of the [directorySettingTemplate](../resources/directorysettingtemplate.md) objects.

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
GET /directorySettingTemplates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/directorySettingTemplates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directorysettingtemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 538

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directorySettingTemplate",
      "id": "c77f7bf1-7bf1-c77f-f17b-7fc7f17b7fc7",
      "deletedDateTime": "2017-01-01T00:00:34.0507931+03:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "values": [
        {
          "@odata.type": "microsoft.graph.settingTemplateValue",
          "name": "Name value",
          "type": "Type value",
          "defaultValue": "Default Value value"
        }
      ]
    }
  ]
}
```

