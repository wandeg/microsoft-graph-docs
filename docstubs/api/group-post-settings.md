---
title: "Add settings"
description: "Add settings by posting to the settings collection."
author: "**TODO: Provide Github Name**"
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
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
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
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|
|values|[settingValue](../resources/settingvalue.md) collection|**TODO: Add Description**|



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
Content-Type: application/json
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
{
  "@odata.type": "#microsoft.graph.directorySetting",
  "id": "ee6c046f-046f-ee6c-6f04-6cee6f046cee",
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

