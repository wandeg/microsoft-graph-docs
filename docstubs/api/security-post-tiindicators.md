---
title: "Add tiIndicators"
description: "Add tiIndicators by posting to the tiIndicators collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add tiIndicators

Namespace: microsoft.graph

Add tiIndicators by posting to the tiIndicators collection.

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
POST /Security/tiIndicators/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [tiIndicator](../resources/tiindicator.md) object.

The following table shows the properties that are required when you create the [tiIndicator](../resources/tiindicator.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|action|Enumeration| Possible values are: `unknown`, `allow`, `block`, `alert`, `unknownFutureValue`.|
|activityGroupNames|String collection||
|additionalInformation|String||
|azureTenantId|String||
|confidence|Int32||
|description|String||
|diamondModel|Enumeration| Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`, `unknownFutureValue`.|
|domainName|String||
|emailEncoding|String||
|emailLanguage|String||
|emailRecipient|String||
|emailSenderAddress|String||
|emailSenderName|String||
|emailSourceDomain|String||
|emailSourceIpAddress|String||
|emailSubject|String||
|emailXMailer|String||
|expirationDateTime|DateTimeOffset||
|externalId|String||
|fileCompileDateTime|DateTimeOffset||
|fileCreatedDateTime|DateTimeOffset||
|fileHashType|Enumeration| Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `unknownFutureValue`.|
|fileHashValue|String||
|fileMutexName|String||
|fileName|String||
|filePacker|String||
|filePath|String||
|fileSize|Int64||
|fileType|String||
|ingestedDateTime|DateTimeOffset||
|isActive|Boolean||
|killChain|String collection||
|knownFalsePositives|String||
|lastReportedDateTime|DateTimeOffset||
|malwareFamilyNames|String collection||
|networkCidrBlock|String||
|networkDestinationAsn|Int32||
|networkDestinationCidrBlock|String||
|networkDestinationIPv4|String||
|networkDestinationIPv6|String||
|networkDestinationPort|Int32||
|networkIPv4|String||
|networkIPv6|String||
|networkPort|Int32||
|networkProtocol|Int32||
|networkSourceAsn|Int32||
|networkSourceCidrBlock|String||
|networkSourceIPv4|String||
|networkSourceIPv6|String||
|networkSourcePort|Int32||
|passiveOnly|Boolean||
|severity|Int32||
|tags|String collection||
|targetProduct|String||
|threatType|String||
|tlpLevel|Enumeration| Possible values are: `unknown`, `white`, `green`, `amber`, `red`, `unknownFutureValue`.|
|url|String||
|userAgent|String||



## Response
If successful, this method returns a `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_tiindicator_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/tiIndicators
Content-type: application/json
Content-length: 2539

{
  "@odata.type": "#microsoft.graph.tiIndicator",
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
  "expirationDateTime": "2016-12-31T23:57:00.3383939+03:00",
  "externalId": "External Id value",
  "fileCompileDateTime": "2017-01-01T00:03:08.636008+03:00",
  "fileCreatedDateTime": "2017-01-01T00:00:09.4254689+03:00",
  "fileHashType": "String",
  "fileHashValue": "File Hash Value value",
  "fileMutexName": "File Mutex Name value",
  "fileName": "File Name value",
  "filePacker": "File Packer value",
  "filePath": "File Path value",
  "fileSize": 8,
  "fileType": "File Type value",
  "ingestedDateTime": "2016-12-31T23:56:54.9324682+03:00",
  "isActive": true,
  "killChain": [
    "Kill Chain value"
  ],
  "knownFalsePositives": "Known False Positives value",
  "lastReportedDateTime": "2017-01-01T00:01:05.5523888+03:00",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiindicator"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2588

{
  "@odata.type": "#microsoft.graph.tiIndicator",
  "id": "7181f6a7-f6a7-7181-a7f6-8171a7f68171",
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
  "expirationDateTime": "2016-12-31T23:57:00.3383939+03:00",
  "externalId": "External Id value",
  "fileCompileDateTime": "2017-01-01T00:03:08.636008+03:00",
  "fileCreatedDateTime": "2017-01-01T00:00:09.4254689+03:00",
  "fileHashType": "String",
  "fileHashValue": "File Hash Value value",
  "fileMutexName": "File Mutex Name value",
  "fileName": "File Name value",
  "filePacker": "File Packer value",
  "filePath": "File Path value",
  "fileSize": 8,
  "fileType": "File Type value",
  "ingestedDateTime": "2016-12-31T23:56:54.9324682+03:00",
  "isActive": true,
  "killChain": [
    "Kill Chain value"
  ],
  "knownFalsePositives": "Known False Positives value",
  "lastReportedDateTime": "2017-01-01T00:01:05.5523888+03:00",
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
```

