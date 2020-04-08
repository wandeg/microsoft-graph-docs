---
title: "macOSKerberosSingleSignOnExtension resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# macOSKerberosSingleSignOnExtension resource type


Namespace: microsoft.graph




Inherits from [macOSSingleSignOnExtension](../resources/macossinglesignonextension.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeDirectorySiteCode|String||
|blockActiveDirectorySiteAutoDiscovery|Boolean||
|blockAutomaticLogin|Boolean||
|cacheName|String||
|credentialBundleIdAccessControlList|String collection||
|domainRealms|String collection||
|domains|String collection||
|isDefaultRealm|Boolean||
|passwordBlockModification|Boolean||
|passwordChangeUrl|String||
|passwordEnableLocalSync|Boolean||
|passwordExpirationDays|Int32||
|passwordExpirationNotificationDays|Int32||
|passwordMinimumAgeDays|Int32||
|passwordMinimumLength|Int32||
|passwordPreviousPasswordBlockCount|Int32||
|passwordRequireActiveDirectoryComplexity|Boolean||
|passwordRequirementsDescription|String||
|realm|String||
|requireUserPresence|Boolean||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKerberosSingleSignOnExtension",
  "realm": "String",
  "domains": [
    "String"
  ],
  "blockAutomaticLogin": true,
  "cacheName": "String",
  "credentialBundleIdAccessControlList": [
    "String"
  ],
  "domainRealms": [
    "String"
  ],
  "isDefaultRealm": true,
  "passwordBlockModification": true,
  "passwordExpirationDays": 1024,
  "passwordExpirationNotificationDays": 1024,
  "userPrincipalName": "String",
  "passwordRequireActiveDirectoryComplexity": true,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumAgeDays": 1024,
  "passwordRequirementsDescription": "String",
  "requireUserPresence": true,
  "activeDirectorySiteCode": "String",
  "passwordEnableLocalSync": true,
  "blockActiveDirectorySiteAutoDiscovery": true,
  "passwordChangeUrl": "String"
}
```

