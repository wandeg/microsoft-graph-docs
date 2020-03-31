---
title: "Get iosManagedAppProtection"
description: "Read properties and relationships of the iosManagedAppProtection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get iosManagedAppProtection

Namespace: microsoft.graph

Read properties and relationships of the [iosManagedAppProtection](../resources/iosmanagedappprotection.md) object.

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
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/iosmanagedappprotection.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_iosmanagedappprotection"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.iosManagedAppProtection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3260

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppProtection",
    "id": "63b2597d-597d-63b2-7d59-b2637d59b263",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
    "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "version": "Version value",
    "periodOfflineBeforeAccessCheck": "-PT3M20.9647168S",
    "periodOnlineBeforeAccessCheck": "PT26.5114428S",
    "allowedInboundDataTransferSources": "String",
    "allowedOutboundDataTransferDestinations": "String",
    "organizationalCredentialsRequired": true,
    "allowedOutboundClipboardSharingLevel": "String",
    "dataBackupBlocked": true,
    "deviceComplianceRequired": true,
    "managedBrowserToOpenLinksRequired": true,
    "saveAsBlocked": true,
    "periodOfflineBeforeWipeIsEnforced": "PT45.0890117S",
    "pinRequired": true,
    "maximumPinRetries": 1,
    "simplePinBlocked": true,
    "minimumPinLength": 0,
    "pinCharacterSet": "String",
    "periodBeforePinReset": "PT2M20.1716074S",
    "allowedDataStorageLocations": [
      "String"
    ],
    "contactSyncBlocked": true,
    "printBlocked": true,
    "fingerprintBlocked": true,
    "disableAppPinIfDevicePinIsSet": true,
    "minimumRequiredOsVersion": "Minimum Required Os Version value",
    "minimumWarningOsVersion": "Minimum Warning Os Version value",
    "minimumRequiredAppVersion": "Minimum Required App Version value",
    "minimumWarningAppVersion": "Minimum Warning App Version value",
    "minimumWipeOsVersion": "Minimum Wipe Os Version value",
    "minimumWipeAppVersion": "Minimum Wipe App Version value",
    "appActionIfDeviceComplianceRequired": "String",
    "appActionIfMaximumPinRetriesExceeded": "String",
    "pinRequiredInsteadOfBiometricTimeout": "PT2M44.7245411S",
    "allowedOutboundClipboardSharingExceptionLength": 14,
    "notificationRestriction": "String",
    "previousPinBlockCount": 5,
    "managedBrowser": "String",
    "maximumAllowedDeviceThreatLevel": "String",
    "mobileThreatDefenseRemediationAction": "String",
    "blockDataIngestionIntoOrganizationDocuments": true,
    "allowedDataIngestionLocations": [
      "String"
    ],
    "appActionIfUnableToAuthenticateUser": "String",
    "isAssigned": true,
    "targetedAppManagementLevels": "String",
    "appDataEncryptionType": "String",
    "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
    "deployedAppCount": 0,
    "faceIdBlocked": true,
    "exemptedAppProtocols": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
    "allowedIosDeviceModels": "Allowed Ios Device Models value",
    "appActionIfIosDeviceModelNotAllowed": "String",
    "thirdPartyKeyboardsBlocked": true,
    "filterOpenInToOnlyManagedApps": true,
    "disableProtectionOfManagedOutboundOpenInData": true,
    "protectInboundDataFromUnknownSources": true,
    "customBrowserProtocol": "Custom Browser Protocol value"
  }
}
```

