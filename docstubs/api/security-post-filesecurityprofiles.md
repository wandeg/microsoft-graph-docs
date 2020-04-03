---
title: "Add fileSecurityProfiles"
description: "Add fileSecurityProfiles by posting to the fileSecurityProfiles collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add fileSecurityProfiles

Namespace: microsoft.graph

Add fileSecurityProfiles by posting to the fileSecurityProfiles collection.

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
POST /Security/fileSecurityProfiles/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [fileSecurityProfile](../resources/filesecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_filesecurityprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/fileSecurityProfiles
Content-type: application/json
Content-length: 1418

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
  "firstSeenDateTime": "2016-12-31T23:57:13.529911+00:00",
  "hashes": [
    {
      "@odata.type": "microsoft.graph.fileHash",
      "hashType": "String",
      "hashValue": "Hash Value value"
    }
  ],
  "lastSeenDateTime": "2016-12-31T23:58:33.6279063+00:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.filesecurityprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1467

{
  "@odata.type": "#microsoft.graph.fileSecurityProfile",
  "id": "fa207c43-7c43-fa20-437c-20fa437c20fa",
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
  "firstSeenDateTime": "2016-12-31T23:57:13.529911+00:00",
  "hashes": [
    {
      "@odata.type": "microsoft.graph.fileHash",
      "hashType": "String",
      "hashValue": "Hash Value value"
    }
  ],
  "lastSeenDateTime": "2016-12-31T23:58:33.6279063+00:00",
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

