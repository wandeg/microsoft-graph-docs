---
title: "Get directorySetting"
description: "Read properties and relationships of a directorySetting object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get directorySetting

Namespace: Microsoft.DirectoryServices

Read properties and relationships of a [directorySetting](../resources/microsoft.directoryservices-directorysetting.md) object.

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
GET /settings/{settingsId}
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
If successful, this method returns a `200 OK` response code and a [directorySetting](../resources/microsoft.directoryservices-directorysetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}
-->
``` http
GET https://graph.microsoft.com/changelog/settings/{settingsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.directorySetting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.DirectoryServices.directorySetting",
    "id": "3e014d50-4d50-3e01-504d-013e504d013e",
    "displayName": "Display Name value",
    "templateId": "Template Id value",
    "values": [
      {
        "@odata.type": "Microsoft.DirectoryServices.settingValue",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```

