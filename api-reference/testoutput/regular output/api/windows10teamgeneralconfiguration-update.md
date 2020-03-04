---
title: "Update windows10TeamGeneralConfiguration"
description: "Update the properties of a windows10TeamGeneralConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update windows10TeamGeneralConfiguration

Namespace: microsoft.graph

Update the properties of a [windows10TeamGeneralConfiguration](../resources/windows10teamgeneralconfiguration.md) object.

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
PATCH ** Entity URI for microsoft.graph.windows10TeamGeneralConfiguration not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/windows10teamgeneralconfiguration.md) object.

The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/windows10teamgeneralconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|azureOperationalInsightsBlockTelemetry|Boolean|Indicates whether or not to Block Azure Operational Insights.|
|azureOperationalInsightsWorkspaceId|String|The Azure Operational Insights workspace id.|
|azureOperationalInsightsWorkspaceKey|String|The Azure Operational Insights Workspace key.|
|connectAppBlockAutoLaunch|Boolean|Specifies whether to automatically launch the Connect app whenever a projection is initiated.|
|maintenanceWindowBlocked|Boolean|Indicates whether or not to Block setting a maintenance window for device updates.|
|maintenanceWindowDurationInHours|Int32|Maintenance window duration for device updates. Valid values 0 to 5|
|maintenanceWindowStartTime|TimeOfDay|Maintenance window start time for device updates.|
|miracastChannel|Enumeration|The channel. Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.|
|miracastBlocked|Boolean|Indicates whether or not to Block wireless projection.|
|miracastRequirePin|Boolean|Indicates whether or not to require a pin for wireless projection.|
|settingsBlockMyMeetingsAndFiles|Boolean|Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.|
|settingsBlockSessionResume|Boolean|Specifies whether to allow the ability to resume a session when the session times out.|
|settingsBlockSigninSuggestions|Boolean|Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.|
|settingsDefaultVolume|Int32|Specifies the default volume value for a new session. Permitted values are 0-100. The default is 45. Valid values 0 to 100|
|settingsScreenTimeoutInMinutes|Int32|Specifies the number of minutes until the Hub screen turns off.|
|settingsSessionTimeoutInMinutes|Int32|Specifies the number of minutes until the session times out.|
|settingsSleepTimeoutInMinutes|Int32|Specifies the number of minutes until the Hub enters sleep mode.|
|welcomeScreenBlockAutomaticWakeUp|Boolean|Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.|
|welcomeScreenBackgroundImageUrl|String|The welcome screen background image URL. The URL must use the HTTPS protocol and return a PNG image.|
|welcomeScreenMeetingInformation|Enumeration|The welcome screen meeting information shown. Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/windows10teamgeneralconfiguration.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_windows10teamgeneralconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.windows10TeamGeneralConfiguration not found
Content-type: application/json
Content-length: 1135

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:58:22.8720000",
  "miracastChannel": "String",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "String"
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
Content-Length: 1307

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "7cce4938-4938-7cce-3849-ce7c3849ce7c",
  "lastModifiedDateTime": "2016-12-31T23:58:55.6908839+03:00",
  "createdDateTime": "2017-01-01T00:01:25.3917672+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:58:22.8720000",
  "miracastChannel": "String",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "String"
}
```

