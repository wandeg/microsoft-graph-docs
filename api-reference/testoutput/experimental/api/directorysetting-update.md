---
title: "Update directorySetting"
description: "Update the properties of a directorySetting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update directorySetting

Namespace: microsoft.graph

Update the properties of a [directorySetting](../resources/directorysetting.md) object.

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
PATCH /settings/{settingsId}
PATCH /groups/{groupsId}/settings/{directorySettingId}
PATCH /me/joinedGroups/{groupId}/settings/{directorySettingId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [directorySetting](../resources/directorysetting.md) object.

The following table shows the properties that are required when you create the [directorySetting](../resources/directorysetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|templateId|String||
|values|[settingValue](../resources/settingvalue.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [directorySetting](../resources/directorysetting.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/settings/{settingsId}
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.directorySetting",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

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
```

