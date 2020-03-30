---
title: "updateTiIndicators"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# updateTiIndicators

Namespace: microsoft.graph



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
POST /Security/tiIndicators/updateTiIndicators
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|value|[tiIndicator](../resources/tiindicator.md) collection||



## Response
If successful, this action returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "tiindicator_updatetiindicators"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/tiIndicators/updateTiIndicators

Content-type: application/json
Content-length: 2894

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "74d895ce-95ce-74d8-ce95-d874ce95d874",
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
      "expirationDateTime": "2016-12-31T23:58:48.8634396+03:00",
      "externalId": "External Id value",
      "fileCompileDateTime": "2017-01-01T00:00:11.2544838+03:00",
      "fileCreatedDateTime": "2016-12-31T23:56:32.5082132+03:00",
      "fileHashType": "String",
      "fileHashValue": "File Hash Value value",
      "fileMutexName": "File Mutex Name value",
      "fileName": "File Name value",
      "filePacker": "File Packer value",
      "filePath": "File Path value",
      "fileSize": 8,
      "fileType": "File Type value",
      "ingestedDateTime": "2016-12-31T23:56:39.7639022+03:00",
      "isActive": true,
      "killChain": [
        "Kill Chain value"
      ],
      "knownFalsePositives": "Known False Positives value",
      "lastReportedDateTime": "2016-12-31T23:59:04.0371883+03:00",
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
      "id": "74d895ce-95ce-74d8-ce95-d874ce95d874",
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
      "expirationDateTime": "2016-12-31T23:58:48.8634396+03:00",
      "externalId": "External Id value",
      "fileCompileDateTime": "2017-01-01T00:00:11.2544838+03:00",
      "fileCreatedDateTime": "2016-12-31T23:56:32.5082132+03:00",
      "fileHashType": "String",
      "fileHashValue": "File Hash Value value",
      "fileMutexName": "File Mutex Name value",
      "fileName": "File Name value",
      "filePacker": "File Packer value",
      "filePath": "File Path value",
      "fileSize": 8,
      "fileType": "File Type value",
      "ingestedDateTime": "2016-12-31T23:56:39.7639022+03:00",
      "isActive": true,
      "killChain": [
        "Kill Chain value"
      ],
      "knownFalsePositives": "Known False Positives value",
      "lastReportedDateTime": "2016-12-31T23:59:04.0371883+03:00",
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

