---
title: "List directorySettingTemplates"
description: "Get a list of the directorySettingTemplate objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List directorySettingTemplates

Namespace: Microsoft.DirectoryServices

Get a list of the [directorySettingTemplate](../resources/directorysettingtemplate.md) objects and their properties.

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
GET /directorySettingTemplates
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
If successful, this method returns a `200 OK` response code and a collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}
-->
``` http
GET https://graph.microsoft.com/changelog/directorySettingTemplates
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.directoryservices.directorysettingtemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.directorySettingTemplate",
      "id": "843c296e-296e-843c-6e29-3c846e293c84",
      "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "values": [
        {
          "@odata.type": "Microsoft.DirectoryServices.settingTemplateValue",
          "name": "Name value",
          "type": "Type value",
          "defaultValue": "Default Value value"
        }
      ]
    }
  ]
}
```

