---
title: "Add settings"
description: "Add settings by posting to the settings collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add settings

Namespace: microsoft.graph

Add settings by posting to the settings collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /groups/{groupsId}/settings/$ref
POST /me/joinedGroups/{groupId}/settings/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and a [directorySetting](../resources/directorysetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/settings
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.directorySetting",
  "id": "3a2582d7-82d7-3a25-d782-253ad782253a",
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

