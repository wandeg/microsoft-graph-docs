---
title: "Update groupSetting"
description: "Update the properties of a groupSetting object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update groupSetting

Namespace: microsoft.graph

Update the properties of a [groupSetting](../resources/groupsetting.md) object.

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
PATCH /groupSettings/{groupSettingsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupSetting](../resources/groupsetting.md) object.

The following table shows the properties that are required when you create the [groupSetting](../resources/groupsetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|
|values|[settingValue](../resources/settingvalue.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [groupSetting](../resources/groupsetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{groupSettingsId}
Content-Type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.groupSetting",
  "displayName": "String",
  "templateId": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingValue"
    }
  ]
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.groupSetting",
  "id": "d1648522-8522-d164-2285-64d1228564d1",
  "displayName": "String",
  "templateId": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingValue"
    }
  ]
}
```

