---
title: "tiIndicator resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# tiIndicator resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get tiIndicator](../api/tiindicator-get.md)|[tiIndicator](../resources/tiIndicator.md)|Read properties and relationships of the [tiIndicator](../resources/tiindicator.md) object.|
|[Delete tiIndicator](../api/tiindicator-delete.md)|None|Deletes a [tiIndicator](../resources/tiindicator.md).|
|[Update tiIndicator](../api/tiindicator-update.md)|[tiIndicator](../resources/tiIndicator.md)|Update the properties of a [tiIndicator](../resources/tiindicator.md) object.|
|[List tiIndicators](../api/security-list-tiindicators.md)|[tiIndicator](../resources/tiIndicator.md) collection|Get the tiIndicators from the tiIndicators navigation property.|
|[Add tiIndicators](../api/security-post-tiindicators.md)|[tiIndicator](../resources/tiIndicator.md)|Add tiIndicators by posting to the tiIndicators collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
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
|id|String| Inherited from [entity](../resources/entity.md)|
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

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tiIndicator",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tiIndicator",
  "id": "String (identifier)",
  "action": "String",
  "activityGroupNames": [
    "String"
  ],
  "additionalInformation": "String",
  "azureTenantId": "String",
  "confidence": 1024,
  "description": "String",
  "diamondModel": "String",
  "domainName": "String",
  "emailEncoding": "String",
  "emailLanguage": "String",
  "emailRecipient": "String",
  "emailSenderAddress": "String",
  "emailSenderName": "String",
  "emailSourceDomain": "String",
  "emailSourceIpAddress": "String",
  "emailSubject": "String",
  "emailXMailer": "String",
  "expirationDateTime": "String (timestamp)",
  "externalId": "String",
  "fileCompileDateTime": "String (timestamp)",
  "fileCreatedDateTime": "String (timestamp)",
  "fileHashType": "String",
  "fileHashValue": "String",
  "fileMutexName": "String",
  "fileName": "String",
  "filePacker": "String",
  "filePath": "String",
  "fileSize": 1024,
  "fileType": "String",
  "ingestedDateTime": "String (timestamp)",
  "isActive": true,
  "killChain": [
    "String"
  ],
  "knownFalsePositives": "String",
  "lastReportedDateTime": "String (timestamp)",
  "malwareFamilyNames": [
    "String"
  ],
  "networkCidrBlock": "String",
  "networkDestinationAsn": 1024,
  "networkDestinationCidrBlock": "String",
  "networkDestinationIPv4": "String",
  "networkDestinationIPv6": "String",
  "networkDestinationPort": 1024,
  "networkIPv4": "String",
  "networkIPv6": "String",
  "networkPort": 1024,
  "networkProtocol": 1024,
  "networkSourceAsn": 1024,
  "networkSourceCidrBlock": "String",
  "networkSourceIPv4": "String",
  "networkSourceIPv6": "String",
  "networkSourcePort": 1024,
  "passiveOnly": true,
  "severity": 1024,
  "tags": [
    "String"
  ],
  "targetProduct": "String",
  "threatType": "String",
  "tlpLevel": "String",
  "url": "String",
  "userAgent": "String"
}
```

