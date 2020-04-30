---
title: "Create directorySetting"
description: "Create a new directorySetting object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create directorySetting

Namespace: Microsoft.DirectoryServices

Create a new [directorySetting](../resources/microsoft.directoryservices-directorysetting.md) object.

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
POST /settings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [directorySetting](../resources/microsoft.directoryservices-directorysetting.md) object.

The following table shows the properties that are required when you create the [directorySetting](../resources/microsoft.directoryservices-directorysetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|
|values|[settingValue](../resources/microsoft.directoryservices-settingvalue.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [directorySetting](../resources/microsoft.directoryservices-directorysetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}
-->
``` http
POST https://graph.microsoft.com/changelog/settings
Content-Type: application/json
Content-length: 308

{
  "@odata.type": "#Microsoft.DirectoryServices.directorySetting",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.directorysetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
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
```

