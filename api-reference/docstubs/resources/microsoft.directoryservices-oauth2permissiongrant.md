---
title: "oAuth2PermissionGrant resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# oAuth2PermissionGrant resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get oAuth2PermissionGrant](../api/microsoft.directoryservices-oauth2permissiongrant-get.md)|[oAuth2PermissionGrant](../resources/microsoft.directoryservices-oauth2permissiongrant.md)|Read properties and relationships of an [oAuth2PermissionGrant](../resources/microsoft.directoryservices-oauth2permissiongrant.md) object.|
|[Update oAuth2PermissionGrant](../api/microsoft.directoryservices-oauth2permissiongrant-update.md)|[oAuth2PermissionGrant](../resources/microsoft.directoryservices-oauth2permissiongrant.md)|Update the properties of a [oAuth2PermissionGrant](../resources/microsoft.directoryservices-oauth2permissiongrant.md) object.|
|[delta](../api/microsoft.directoryservices-oauth2permissiongrant-delta.md)|[oAuth2PermissionGrant](../resources/microsoft.directoryservices-oauth2permissiongrant.md) collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientId|String|**TODO: Add Description**|
|consentType|String|**TODO: Add Description**|
|expiryTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|principalId|String|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|scope|String|**TODO: Add Description**|
|startTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.oAuth2PermissionGrant",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.oAuth2PermissionGrant",
  "clientId": "String",
  "consentType": "String",
  "expiryTime": "String (timestamp)",
  "id": "String (identifier)",
  "principalId": "String",
  "resourceId": "String",
  "scope": "String",
  "startTime": "String (timestamp)"
}
```

