---
title: "List settings"
description: "Get the directorySettings from the settings navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List settings

Namespace: microsoft.graph

Get the directorySettings from the settings navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /groups/{groupsId}/settings
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [directorySetting](../resources/directorysetting.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/groups/{groupsId}/settings
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directorysetting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directorySetting",
      "id": "aaf01c3d-1c3d-aaf0-3d1c-f0aa3d1cf0aa",
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

