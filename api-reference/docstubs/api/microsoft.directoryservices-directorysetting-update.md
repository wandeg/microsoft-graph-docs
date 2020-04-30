---
title: "Update directorySetting"
description: "Update the properties of a directorySetting object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update directorySetting

Namespace: Microsoft.DirectoryServices

Update the properties of a [directorySetting](../resources/microsoft.directoryservices-directorysetting.md) object.

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
PATCH /settings/{settingsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

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
If successful, this method returns a `200 OK` response code and an updated [directorySetting](../resources/microsoft.directoryservices-directorysetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/settings/{settingsId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
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

