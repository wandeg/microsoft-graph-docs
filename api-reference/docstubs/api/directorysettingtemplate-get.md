---
title: "Get directorySettingTemplate"
description: "Read properties and relationships of the directorySettingTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get directorySettingTemplate

Namespace: microsoft.graph

Read properties and relationships of the [directorySettingTemplate](../resources/directorysettingtemplate.md) object.

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
GET /directorySettingTemplates/{directorySettingTemplatesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{directorySettingTemplatesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 498

{
  "value": {
    "@odata.type": "#microsoft.graph.directorySettingTemplate",
    "id": "049cd9b5-d9b5-049c-b5d9-9c04b5d99c04",
    "deletedDateTime": "2017-01-01T00:02:56.4302403+03:00",
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
}
```

