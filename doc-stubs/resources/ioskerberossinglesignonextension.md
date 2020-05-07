---
title: "iosKerberosSingleSignOnExtension resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# iosKerberosSingleSignOnExtension resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [iosSingleSignOnExtension](../resources/iossinglesignonextension.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeDirectorySiteCode|String|**TODO: Add Description**|
|blockActiveDirectorySiteAutoDiscovery|Boolean|**TODO: Add Description**|
|blockAutomaticLogin|Boolean|**TODO: Add Description**|
|cacheName|String|**TODO: Add Description**|
|credentialBundleIdAccessControlList|String collection|**TODO: Add Description**|
|domainRealms|String collection|**TODO: Add Description**|
|domains|String collection|**TODO: Add Description**|
|isDefaultRealm|Boolean|**TODO: Add Description**|
|passwordBlockModification|Boolean|**TODO: Add Description**|
|passwordChangeUrl|String|**TODO: Add Description**|
|passwordEnableLocalSync|Boolean|**TODO: Add Description**|
|passwordExpirationDays|Int32|**TODO: Add Description**|
|passwordExpirationNotificationDays|Int32|**TODO: Add Description**|
|passwordMinimumAgeDays|Int32|**TODO: Add Description**|
|passwordMinimumLength|Int32|**TODO: Add Description**|
|passwordPreviousPasswordBlockCount|Int32|**TODO: Add Description**|
|passwordRequireActiveDirectoryComplexity|Boolean|**TODO: Add Description**|
|passwordRequirementsDescription|String|**TODO: Add Description**|
|realm|String|**TODO: Add Description**|
|requireUserPresence|Boolean|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosKerberosSingleSignOnExtension",
  "realm": "String",
  "domains": [
    "String"
  ],
  "blockAutomaticLogin": "Boolean",
  "cacheName": "String",
  "credentialBundleIdAccessControlList": [
    "String"
  ],
  "domainRealms": [
    "String"
  ],
  "isDefaultRealm": "Boolean",
  "passwordBlockModification": "Boolean",
  "passwordExpirationDays": "Integer",
  "passwordExpirationNotificationDays": "Integer",
  "userPrincipalName": "String",
  "passwordRequireActiveDirectoryComplexity": "Boolean",
  "passwordPreviousPasswordBlockCount": "Integer",
  "passwordMinimumLength": "Integer",
  "passwordMinimumAgeDays": "Integer",
  "passwordRequirementsDescription": "String",
  "requireUserPresence": "Boolean",
  "activeDirectorySiteCode": "String",
  "passwordEnableLocalSync": "Boolean",
  "blockActiveDirectorySiteAutoDiscovery": "Boolean",
  "passwordChangeUrl": "String"
}
```

