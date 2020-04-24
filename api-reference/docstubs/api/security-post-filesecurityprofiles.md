---
title: "Create fileSecurityProfiles"
description: "Create a new fileSecurityProfiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create fileSecurityProfiles

Namespace: microsoft.graph

Create a new fileSecurityProfiles object.

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
POST /Security/fileSecurityProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [fileSecurityProfile](../resources/filesecurityprofile.md) object.

The following table shows the properties that are required when you create the [fileSecurityProfile](../resources/filesecurityprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activityGroupNames|String collection|**TODO: Add Description**|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|certificateThumbprint|String|**TODO: Add Description**|
|extensions|String collection|**TODO: Add Description**|
|fileType|String|**TODO: Add Description**|
|firstSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|hashes|[fileHash](../resources/filehash.md) collection|**TODO: Add Description**|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|malwareStates|[malwareState](../resources/malwarestate.md) collection|**TODO: Add Description**|
|names|String collection|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|
|size|Int64|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|
|vulnerabilityStates|[vulnerabilityState](../resources/vulnerabilitystate.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [fileSecurityProfile](../resources/filesecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_filesecurityprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/fileSecurityProfiles
Content-Type: application/json
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
  "firstSeenDateTime": "2016-12-31T23:56:24.2596319+03:00",
  "hashes": [
    {
      "@odata.type": "microsoft.graph.fileHash",
      "hashType": "String",
      "hashValue": "Hash Value value"
    }
  ],
  "lastSeenDateTime": "2017-01-01T00:02:18.945458+03:00",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.filesecurityprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.fileSecurityProfile",
  "id": "242c3c91-3c91-242c-913c-2c24913c2c24",
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
  "firstSeenDateTime": "2016-12-31T23:56:24.2596319+03:00",
  "hashes": [
    {
      "@odata.type": "microsoft.graph.fileHash",
      "hashType": "String",
      "hashValue": "Hash Value value"
    }
  ],
  "lastSeenDateTime": "2017-01-01T00:02:18.945458+03:00",
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

