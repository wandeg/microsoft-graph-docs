---
title: "Update fileSecurityProfile"
description: "Update the properties of a fileSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update fileSecurityProfile

Namespace: microsoft.graph

Update the properties of a [fileSecurityProfile](../resources/filesecurityprofile.md) object.

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
PATCH /Security/fileSecurityProfiles/{fileSecurityProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [fileSecurityProfile](../resources/filesecurityprofile.md) object.

The following table shows the properties that are required when you create the [fileSecurityProfile](../resources/filesecurityprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activityGroupNames|String collection||
|azureSubscriptionId|String||
|azureTenantId|String||
|certificateThumbprint|String||
|extensions|String collection||
|fileType|String||
|firstSeenDateTime|DateTimeOffset||
|hashes|[fileHash](../resources/filehash.md) collection||
|lastSeenDateTime|DateTimeOffset||
|malwareStates|[malwareState](../resources/malwarestate.md) collection||
|names|String collection||
|riskScore|String||
|size|Int64||
|tags|String collection||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||
|vulnerabilityStates|[vulnerabilityState](../resources/vulnerabilitystate.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [fileSecurityProfile](../resources/filesecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_filesecurityprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/fileSecurityProfiles/{fileSecurityProfileId}
Content-type: application/json
Content-length: 1419

{
  "@odata.type": "#microsoft.graph.fileSecurityProfile",
  "activityGroupNames": [
    "Activity Group Names value"
  ],
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "extensions": [
    "Extensions value"
  ],
  "fileType": "File Type value",
  "firstSeenDateTime": "2017-01-01T00:02:25.6939099+00:00",
  "hashes": [
    {
      "@odata.type": "microsoft.graph.fileHash",
      "hashType": "String",
      "hashValue": "Hash Value value"
    }
  ],
  "lastSeenDateTime": "2017-01-01T00:01:32.8955884+00:00",
  "malwareStates": [
    {
      "@odata.type": "microsoft.graph.malwareState",
      "category": "Category value",
      "family": "Family value",
      "name": "Name value",
      "severity": "Severity value",
      "wasRunning": true
    }
  ],
  "names": [
    "Names value"
  ],
  "riskScore": "Risk Score value",
  "size": 4,
  "tags": [
    "Tags value"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  },
  "vulnerabilityStates": [
    {
      "@odata.type": "microsoft.graph.vulnerabilityState",
      "cve": "Cve value"
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1468

{
  "@odata.type": "#microsoft.graph.fileSecurityProfile",
  "id": "6ff0b94c-b94c-6ff0-4cb9-f06f4cb9f06f",
  "activityGroupNames": [
    "Activity Group Names value"
  ],
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "extensions": [
    "Extensions value"
  ],
  "fileType": "File Type value",
  "firstSeenDateTime": "2017-01-01T00:02:25.6939099+00:00",
  "hashes": [
    {
      "@odata.type": "microsoft.graph.fileHash",
      "hashType": "String",
      "hashValue": "Hash Value value"
    }
  ],
  "lastSeenDateTime": "2017-01-01T00:01:32.8955884+00:00",
  "malwareStates": [
    {
      "@odata.type": "microsoft.graph.malwareState",
      "category": "Category value",
      "family": "Family value",
      "name": "Name value",
      "severity": "Severity value",
      "wasRunning": true
    }
  ],
  "names": [
    "Names value"
  ],
  "riskScore": "Risk Score value",
  "size": 4,
  "tags": [
    "Tags value"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  },
  "vulnerabilityStates": [
    {
      "@odata.type": "microsoft.graph.vulnerabilityState",
      "cve": "Cve value"
    }
  ]
}
```

