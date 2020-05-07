---
title: "Get androidManagedAppProtection"
description: "Read the properties and relationships of an androidManagedAppProtection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get androidManagedAppProtection

Namespace: microsoft.graph

Read the properties and relationships of an [androidManagedAppProtection](../resources/androidmanagedappprotection.md) object.

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
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [androidManagedAppProtection](../resources/androidmanagedappprotection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_androidmanagedappprotection"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidManagedAppProtection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedAppProtection",
    "id": "871f8125-8125-871f-2581-1f8725811f87",
    "displayName": "String",
    "description": "String",
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "roleScopeTagIds": [
      "String"
    ],
    "version": "String",
    "periodOfflineBeforeAccessCheck": "String (duration)",
    "periodOnlineBeforeAccessCheck": "String (duration)",
    "allowedInboundDataTransferSources": "String",
    "allowedOutboundDataTransferDestinations": "String",
    "organizationalCredentialsRequired": "Boolean",
    "allowedOutboundClipboardSharingLevel": "String",
    "dataBackupBlocked": "Boolean",
    "deviceComplianceRequired": "Boolean",
    "managedBrowserToOpenLinksRequired": "Boolean",
    "saveAsBlocked": "Boolean",
    "periodOfflineBeforeWipeIsEnforced": "String (duration)",
    "pinRequired": "Boolean",
    "maximumPinRetries": "Integer",
    "simplePinBlocked": "Boolean",
    "minimumPinLength": "Integer",
    "pinCharacterSet": "String",
    "periodBeforePinReset": "String (duration)",
    "allowedDataStorageLocations": [
      "String"
    ],
    "contactSyncBlocked": "Boolean",
    "printBlocked": "Boolean",
    "fingerprintBlocked": "Boolean",
    "disableAppPinIfDevicePinIsSet": "Boolean",
    "minimumRequiredOsVersion": "String",
    "minimumWarningOsVersion": "String",
    "minimumRequiredAppVersion": "String",
    "minimumWarningAppVersion": "String",
    "minimumWipeOsVersion": "String",
    "minimumWipeAppVersion": "String",
    "appActionIfDeviceComplianceRequired": "String",
    "appActionIfMaximumPinRetriesExceeded": "String",
    "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
    "allowedOutboundClipboardSharingExceptionLength": "Integer",
    "notificationRestriction": "String",
    "previousPinBlockCount": "Integer",
    "managedBrowser": "String",
    "maximumAllowedDeviceThreatLevel": "String",
    "mobileThreatDefenseRemediationAction": "String",
    "blockDataIngestionIntoOrganizationDocuments": "Boolean",
    "allowedDataIngestionLocations": [
      "String"
    ],
    "appActionIfUnableToAuthenticateUser": "String",
    "isAssigned": "Boolean",
    "targetedAppManagementLevels": "String",
    "screenCaptureBlocked": "Boolean",
    "disableAppEncryptionIfDeviceEncryptionIsEnabled": "Boolean",
    "encryptAppData": "Boolean",
    "deployedAppCount": "Integer",
    "minimumRequiredPatchVersion": "String",
    "minimumWarningPatchVersion": "String",
    "exemptedAppPackages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair"
      }
    ],
    "minimumWipePatchVersion": "String",
    "allowedAndroidDeviceManufacturers": "String",
    "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
    "requiredAndroidSafetyNetDeviceAttestationType": "String",
    "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
    "requiredAndroidSafetyNetAppsVerificationType": "String",
    "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
    "customBrowserPackageId": "String",
    "customBrowserDisplayName": "String",
    "minimumRequiredCompanyPortalVersion": "String",
    "minimumWarningCompanyPortalVersion": "String",
    "minimumWipeCompanyPortalVersion": "String",
    "keyboardsRestricted": "Boolean",
    "approvedKeyboards": [
      {
        "@odata.type": "microsoft.graph.keyValuePair"
      }
    ],
    "allowedAndroidDeviceModels": [
      "String"
    ],
    "appActionIfAndroidDeviceModelNotAllowed": "String"
  }
}
```

