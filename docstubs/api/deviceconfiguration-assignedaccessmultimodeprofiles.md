---
title: "assignedAccessMultiModeProfiles"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# assignedAccessMultiModeProfiles

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|assignedAccessMultiModeProfiles|[windowsAssignedAccessProfile](../resources/windowsassignedaccessprofile.md) collection||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "deviceconfiguration_assignedaccessmultimodeprofiles"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles

Content-type: application/json
Content-length: 528

{
  "assignedAccessMultiModeProfiles": [
    {
      "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
      "id": "0262cead-cead-0262-adce-6202adce6202",
      "profileName": "Profile Name value",
      "showTaskBar": true,
      "appUserModelIds": [
        "App User Model Ids value"
      ],
      "desktopAppPaths": [
        "Desktop App Paths value"
      ],
      "userAccounts": [
        "User Accounts value"
      ],
      "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
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

