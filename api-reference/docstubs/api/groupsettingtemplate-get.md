---
title: "Get groupSettingTemplate"
description: "Read properties and relationships of a groupSettingTemplate object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get groupSettingTemplate

Namespace: microsoft.graph

Read properties and relationships of a [groupSettingTemplate](../resources/groupsettingtemplate.md) object.

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
GET /groupSettingTemplates/{groupSettingTemplatesId}
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
If successful, this method returns a `200 OK` response code and a [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/groupSettingTemplates/{groupSettingTemplatesId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.groupSettingTemplate",
    "id": "3c8bd7e4-d7e4-3c8b-e4d7-8b3ce4d78b3c",
    "deletedDateTime": "2016-12-31T23:57:29.5624424+00:00",
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

