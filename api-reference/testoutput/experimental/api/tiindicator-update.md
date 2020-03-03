---
title: "Update tiIndicator"
description: "Update the properties of a tiIndicator object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update tiIndicator

Namespace: microsoft.graph

Update the properties of a [tiIndicator](../resources/tiindicator.md) object.

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
PATCH /Security/tiIndicators/{tiIndicatorId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [tiIndicator](../resources/tiindicator.md) object.

The following table shows the properties that are required when you create the [tiIndicator](../resources/tiindicator.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|action|Enumeration|. Possible values are: `unknown`, `allow`, `block`, `alert`, `unknownFutureValue`.|
|activityGroupNames|String collection||
|additionalInformation|String||
|azureTenantId|String||
|confidence|Int32||
|description|String||
|diamondModel|Enumeration|. Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`, `unknownFutureValue`.|
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
|fileHashType|Enumeration|. Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `unknownFutureValue`.|
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
|tlpLevel|Enumeration|. Possible values are: `unknown`, `white`, `green`, `amber`, `red`, `unknownFutureValue`.|
|url|String||
|userAgent|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [tiIndicator](../resources/tiindicator.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_tiindicator"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/Security/tiIndicators/{tiIndicatorId}
Content-type: application/json
Content-length: 2540

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
  "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
  "externalId": "External Id value",
  "fileCompileDateTime": "2017-01-01T00:02:30.4914742+03:00",
  "fileCreatedDateTime": "2016-12-31T23:56:41.8083525+03:00",
  "fileHashType": "String",
  "fileHashValue": "File Hash Value value",
  "fileMutexName": "File Mutex Name value",
  "fileName": "File Name value",
  "filePacker": "File Packer value",
  "filePath": "File Path value",
  "fileSize": 8,
  "fileType": "File Type value",
  "ingestedDateTime": "2017-01-01T00:02:21.7613669+03:00",
  "isActive": true,
  "killChain": [
    "Kill Chain value"
  ],
  "knownFalsePositives": "Known False Positives value",
  "lastReportedDateTime": "2017-01-01T00:01:11.3421719+03:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2589

{
  "@odata.type": "#microsoft.graph.tiIndicator",
  "id": "ebcb7b71-7b71-ebcb-717b-cbeb717bcbeb",
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
  "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
  "externalId": "External Id value",
  "fileCompileDateTime": "2017-01-01T00:02:30.4914742+03:00",
  "fileCreatedDateTime": "2016-12-31T23:56:41.8083525+03:00",
  "fileHashType": "String",
  "fileHashValue": "File Hash Value value",
  "fileMutexName": "File Mutex Name value",
  "fileName": "File Name value",
  "filePacker": "File Packer value",
  "filePath": "File Path value",
  "fileSize": 8,
  "fileType": "File Type value",
  "ingestedDateTime": "2017-01-01T00:02:21.7613669+03:00",
  "isActive": true,
  "killChain": [
    "Kill Chain value"
  ],
  "knownFalsePositives": "Known False Positives value",
  "lastReportedDateTime": "2017-01-01T00:01:11.3421719+03:00",
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

