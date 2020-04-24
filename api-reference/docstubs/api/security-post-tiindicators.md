---
title: "Create tiIndicators"
description: "Create a new tiIndicators object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create tiIndicators

Namespace: microsoft.graph

Create a new tiIndicators object.

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
POST /Security/tiIndicators
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [tiIndicator](../resources/tiindicator.md) object.

The following table shows the properties that are required when you create the [tiIndicator](../resources/tiindicator.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|action|tiAction|**TODO: Add Description**. Possible values are: `unknown`, `allow`, `block`, `alert`, `unknownFutureValue`.|
|activityGroupNames|String collection|**TODO: Add Description**|
|additionalInformation|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|confidence|Int32|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|diamondModel|diamondModel|**TODO: Add Description**. Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`, `unknownFutureValue`.|
|domainName|String|**TODO: Add Description**|
|emailEncoding|String|**TODO: Add Description**|
|emailLanguage|String|**TODO: Add Description**|
|emailRecipient|String|**TODO: Add Description**|
|emailSenderAddress|String|**TODO: Add Description**|
|emailSenderName|String|**TODO: Add Description**|
|emailSourceDomain|String|**TODO: Add Description**|
|emailSourceIpAddress|String|**TODO: Add Description**|
|emailSubject|String|**TODO: Add Description**|
|emailXMailer|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|fileCompileDateTime|DateTimeOffset|**TODO: Add Description**|
|fileCreatedDateTime|DateTimeOffset|**TODO: Add Description**|
|fileHashType|fileHashType|**TODO: Add Description**. Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `unknownFutureValue`.|
|fileHashValue|String|**TODO: Add Description**|
|fileMutexName|String|**TODO: Add Description**|
|fileName|String|**TODO: Add Description**|
|filePacker|String|**TODO: Add Description**|
|filePath|String|**TODO: Add Description**|
|fileSize|Int64|**TODO: Add Description**|
|fileType|String|**TODO: Add Description**|
|ingestedDateTime|DateTimeOffset|**TODO: Add Description**|
|isActive|Boolean|**TODO: Add Description**|
|killChain|String collection|**TODO: Add Description**|
|knownFalsePositives|String|**TODO: Add Description**|
|lastReportedDateTime|DateTimeOffset|**TODO: Add Description**|
|malwareFamilyNames|String collection|**TODO: Add Description**|
|networkCidrBlock|String|**TODO: Add Description**|
|networkDestinationAsn|Int32|**TODO: Add Description**|
|networkDestinationCidrBlock|String|**TODO: Add Description**|
|networkDestinationIPv4|String|**TODO: Add Description**|
|networkDestinationIPv6|String|**TODO: Add Description**|
|networkDestinationPort|Int32|**TODO: Add Description**|
|networkIPv4|String|**TODO: Add Description**|
|networkIPv6|String|**TODO: Add Description**|
|networkPort|Int32|**TODO: Add Description**|
|networkProtocol|Int32|**TODO: Add Description**|
|networkSourceAsn|Int32|**TODO: Add Description**|
|networkSourceCidrBlock|String|**TODO: Add Description**|
|networkSourceIPv4|String|**TODO: Add Description**|
|networkSourceIPv6|String|**TODO: Add Description**|
|networkSourcePort|Int32|**TODO: Add Description**|
|passiveOnly|Boolean|**TODO: Add Description**|
|severity|Int32|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|targetProduct|String|**TODO: Add Description**|
|threatType|String|**TODO: Add Description**|
|tlpLevel|tlpLevel|**TODO: Add Description**. Possible values are: `unknown`, `white`, `green`, `amber`, `red`, `unknownFutureValue`.|
|url|String|**TODO: Add Description**|
|userAgent|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_tiindicator_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/tiIndicators
Content-Type: application/json
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
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "externalId": "External Id value",
  "fileCompileDateTime": "2017-01-01T00:01:38.3205632+03:00",
  "fileCreatedDateTime": "2017-01-01T00:00:24.2593871+03:00",
  "fileHashType": "String",
  "fileHashValue": "File Hash Value value",
  "fileMutexName": "File Mutex Name value",
  "fileName": "File Name value",
  "filePacker": "File Packer value",
  "filePath": "File Path value",
  "fileSize": 8,
  "fileType": "File Type value",
  "ingestedDateTime": "2017-01-01T00:02:43.9575925+03:00",
  "isActive": true,
  "killChain": [
    "Kill Chain value"
  ],
  "knownFalsePositives": "Known False Positives value",
  "lastReportedDateTime": "2017-01-01T00:00:59.8078557+03:00",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiindicator"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.tiIndicator",
  "id": "efad1db4-1db4-efad-b41d-adefb41dadef",
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
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "externalId": "External Id value",
  "fileCompileDateTime": "2017-01-01T00:01:38.3205632+03:00",
  "fileCreatedDateTime": "2017-01-01T00:00:24.2593871+03:00",
  "fileHashType": "String",
  "fileHashValue": "File Hash Value value",
  "fileMutexName": "File Mutex Name value",
  "fileName": "File Name value",
  "filePacker": "File Packer value",
  "filePath": "File Path value",
  "fileSize": 8,
  "fileType": "File Type value",
  "ingestedDateTime": "2017-01-01T00:02:43.9575925+03:00",
  "isActive": true,
  "killChain": [
    "Kill Chain value"
  ],
  "knownFalsePositives": "Known False Positives value",
  "lastReportedDateTime": "2017-01-01T00:00:59.8078557+03:00",
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

