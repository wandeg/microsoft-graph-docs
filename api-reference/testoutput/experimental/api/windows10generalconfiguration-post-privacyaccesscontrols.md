---
title: "Add privacyAccessControls"
description: "Add privacyAccessControls by posting to the privacyAccessControls collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add privacyAccessControls

Namespace: microsoft.graph

Add privacyAccessControls by posting to the privacyAccessControls collection.

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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md) object.

The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|accessLevel|Enumeration|This indicates an access level for the privacy data category to which the specified application will be given to. Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.|
|dataCategory|Enumeration|This indicates a privacy data category to which the specific access control will apply. Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.|
|appPackageFamilyName|String|The Package Family Name of a Windows app. When set, the access level applies to the specified application.|
|appDisplayName|String|The Package Family Name of a Windows app. When set, the access level applies to the specified application.|



## Response
If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_windowsprivacydataaccesscontrolitem_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
Content-type: application/json
Content-length: 241

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "accessLevel": "String",
  "dataCategory": "String",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsprivacydataaccesscontrolitem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 290

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "6126bcaf-bcaf-6126-afbc-2661afbc2661",
  "accessLevel": "String",
  "dataCategory": "String",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

