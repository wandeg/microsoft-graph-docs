---
title: "windowsPrivacyAccessControls"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# windowsPrivacyAccessControls



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
POST ** Entity URI for microsoft.graph.androidGeneralDeviceConfiguration not found/windowsPrivacyAccessControls
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|windowsPrivacyAccessControls|[windowsPrivacyDataAccessControlItem](../resources/windowsPrivacyDataAccessControlItem.md) collection||



## Response
If successful, this action returns a `204 No Content` response code.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "androidgeneraldeviceconfiguration_windowsprivacyaccesscontrols"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.androidGeneralDeviceConfiguration not found/windowsPrivacyAccessControls

Content-type: application/json
Content-length: 370

{
  "windowsPrivacyAccessControls": [
    {
      "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
      "id": "c2534b6b-4b6b-c253-6b4b-53c26b4b53c2",
      "accessLevel": "String",
      "dataCategory": "String",
      "appPackageFamilyName": "App Package Family Name value",
      "appDisplayName": "App Display Name value"
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
HTTP/1.1 204 No Content
```

