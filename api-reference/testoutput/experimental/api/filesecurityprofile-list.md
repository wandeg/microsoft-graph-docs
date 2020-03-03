---
title: "List fileSecurityProfiles"
description: "List properties and relationships of the fileSecurityProfile objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List fileSecurityProfiles

Namespace: microsoft.graph

List properties and relationships of the [fileSecurityProfile](../resources/filesecurityprofile.md) objects.

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
GET /Security/fileSecurityProfiles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [fileSecurityProfile](../resources/filesecurityprofile.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_filesecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/localtest/Security/fileSecurityProfiles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.filesecurityprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1708

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.fileSecurityProfile",
      "id": "55b90364-0364-55b9-6403-b9556403b955",
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
      "firstSeenDateTime": "2016-12-31T23:57:18.6460025+03:00",
      "hashes": [
        {
          "@odata.type": "microsoft.graph.fileHash",
          "hashType": "String",
          "hashValue": "Hash Value value"
        }
      ],
      "lastSeenDateTime": "2016-12-31T23:59:38.861959+03:00",
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
  ]
}
```

