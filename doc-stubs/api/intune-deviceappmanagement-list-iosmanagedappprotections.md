---
title: "List iosManagedAppProtections"
description: "Get the iosManagedAppProtections from the iosManagedAppProtections navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List iosManagedAppProtections

Namespace: microsoft.graph

Get the iosManagedAppProtections from the iosManagedAppProtections navigation property.

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
GET /deviceAppManagement/iosManagedAppProtections
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

If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/iosmanagedappprotection.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_iosmanagedappprotection"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.iosmanagedappprotection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppProtection",
      "id": "6c8d56e8-56e8-6c8d-e856-8d6ce8568d6c",
      "displayName": "String",
      "description": "String",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
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
      "managedBrowser": "String",
      "isAssigned": "Boolean",
      "appDataEncryptionType": "String",
      "minimumRequiredSdkVersion": "String",
      "deployedAppCount": "Integer",
      "faceIdBlocked": "Boolean",
      "customBrowserProtocol": "String"
    }
  ]
}
```

