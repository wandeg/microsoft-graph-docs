---
title: "Get fileSecurityProfile"
description: "Read properties and relationships of the fileSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get fileSecurityProfile

Namespace: microsoft.graph

Read properties and relationships of the [fileSecurityProfile](../resources/filesecurityprofile.md) object.

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
GET /Security/fileSecurityProfiles/{fileSecurityProfileId}
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
If successful, this method returns a `200 OK` response code and [fileSecurityProfile](../resources/filesecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_filesecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/fileSecurityProfiles/{fileSecurityProfileId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileSecurityProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1591

{
  "value": {
    "@odata.type": "#microsoft.graph.fileSecurityProfile",
    "id": "279c9905-9905-279c-0599-9c2705999c27",
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
    "firstSeenDateTime": "2016-12-31T23:56:26.9196629+00:00",
    "hashes": [
      {
        "@odata.type": "microsoft.graph.fileHash",
        "hashType": "String",
        "hashValue": "Hash Value value"
      }
    ],
    "lastSeenDateTime": "2017-01-01T00:01:38.8802524+00:00",
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
}
```

