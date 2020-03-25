---
title: "List iosManagedAppProtections"
description: "Get the iosManagedAppProtections from the iosManagedAppProtections navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List iosManagedAppProtections

Namespace: microsoft.graph

Get the iosManagedAppProtections from the iosManagedAppProtections navigation property.

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
GET /deviceAppManagement/iosManagedAppProtections
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
If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/iosmanagedappprotection.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_iosmanagedappprotection"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.iosmanagedappprotection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1874

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppProtection",
      "id": "534f83c6-83c6-534f-c683-4f53c6834f53",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:01:12.6625387+03:00",
      "lastModifiedDateTime": "2016-12-31T23:57:04.6185814+03:00",
      "version": "Version value",
      "periodOfflineBeforeAccessCheck": "PT1M34.2461368S",
      "periodOnlineBeforeAccessCheck": "PT6.2198323S",
      "allowedInboundDataTransferSources": "String",
      "allowedOutboundDataTransferDestinations": "String",
      "organizationalCredentialsRequired": true,
      "allowedOutboundClipboardSharingLevel": "String",
      "dataBackupBlocked": true,
      "deviceComplianceRequired": true,
      "managedBrowserToOpenLinksRequired": true,
      "saveAsBlocked": true,
      "periodOfflineBeforeWipeIsEnforced": "-PT3M5.8866192S",
      "pinRequired": true,
      "maximumPinRetries": 1,
      "simplePinBlocked": true,
      "minimumPinLength": 0,
      "pinCharacterSet": "String",
      "periodBeforePinReset": "-PT58.1773705S",
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
      "isAssigned": true,
      "appDataEncryptionType": "String",
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "deployedAppCount": 0,
      "faceIdBlocked": true
    }
  ]
}
```

