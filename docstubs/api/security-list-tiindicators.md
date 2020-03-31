---
title: "List tiIndicators"
description: "Get the tiIndicators from the tiIndicators navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List tiIndicators

Namespace: microsoft.graph

Get the tiIndicators from the tiIndicators navigation property.

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
GET /Security/tiIndicators
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
If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/tiIndicators
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.tiindicator)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2894

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "03cfe201-e201-03cf-01e2-cf0301e2cf03",
      "action": "String",
      "activityGroupNames": [
        "Activity Group Names value"
      ],
      "additionalInformation": "Additional Information value",
      "azureTenantId": "Azure Tenant Id value",
      "confidence": 10,
      "description": "Description value",
      "diamondModel": "String",
      "domainName": "Domain Name value",
      "emailEncoding": "Email Encoding value",
      "emailLanguage": "Email Language value",
      "emailRecipient": "Email Recipient value",
      "emailSenderAddress": "Email Sender Address value",
      "emailSenderName": "Email Sender Name value",
      "emailSourceDomain": "Email Source Domain value",
      "emailSourceIpAddress": "Email Source Ip Address value",
      "emailSubject": "Email Subject value",
      "emailXMailer": "Email XMailer value",
      "expirationDateTime": "2016-12-31T23:58:22.4982594+03:00",
      "externalId": "External Id value",
      "fileCompileDateTime": "2016-12-31T23:56:36.9596494+03:00",
      "fileCreatedDateTime": "2017-01-01T00:02:25.8169251+03:00",
      "fileHashType": "String",
      "fileHashValue": "File Hash Value value",
      "fileMutexName": "File Mutex Name value",
      "fileName": "File Name value",
      "filePacker": "File Packer value",
      "filePath": "File Path value",
      "fileSize": 8,
      "fileType": "File Type value",
      "ingestedDateTime": "2016-12-31T23:59:47.8179253+03:00",
      "isActive": true,
      "killChain": [
        "Kill Chain value"
      ],
      "knownFalsePositives": "Known False Positives value",
      "lastReportedDateTime": "2016-12-31T23:59:02.2314971+03:00",
      "malwareFamilyNames": [
        "Malware Family Names value"
      ],
      "networkCidrBlock": "Network Cidr Block value",
      "networkDestinationAsn": 5,
      "networkDestinationCidrBlock": "Network Destination Cidr Block value",
      "networkDestinationIPv4": "Network Destination IPv4 value",
      "networkDestinationIPv6": "Network Destination IPv6 value",
      "networkDestinationPort": 6,
      "networkIPv4": "Network IPv4 value",
      "networkIPv6": "Network IPv6 value",
      "networkPort": 11,
      "networkProtocol": 15,
      "networkSourceAsn": 0,
      "networkSourceCidrBlock": "Network Source Cidr Block value",
      "networkSourceIPv4": "Network Source IPv4 value",
      "networkSourceIPv6": "Network Source IPv6 value",
      "networkSourcePort": 1,
      "passiveOnly": true,
      "severity": 8,
      "tags": [
        "Tags value"
      ],
      "targetProduct": "Target Product value",
      "threatType": "Threat Type value",
      "tlpLevel": "String",
      "url": "Url value",
      "userAgent": "User Agent value"
    }
  ]
}
```

