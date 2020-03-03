---
title: "windowsPrivacyDataAccessControlItem resource type"
description: "Specify access control level per privacy data category"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsPrivacyDataAccessControlItem resource type


Namespace: microsoft.graph

Specify access control level per privacy data category


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsPrivacyDataAccessControlItems](../api/windowsprivacydataaccesscontrolitem-list.md)|[windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md) collection|List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md) objects.|
|[Get windowsPrivacyDataAccessControlItem](../api/windowsprivacydataaccesscontrolitem-get.md)|[windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md)|Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md) object.|
|[Create windowsPrivacyDataAccessControlItem](../api/windowsprivacydataaccesscontrolitem-create.md)|[windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md)|Create a new [windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md) object.|
|[Delete windowsPrivacyDataAccessControlItem](../api/windowsprivacydataaccesscontrolitem-delete.md)|None|Deletes a [windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md).|
|[Update windowsPrivacyDataAccessControlItem](../api/windowsprivacydataaccesscontrolitem-update.md)|[windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md)|Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/windowsprivacydataaccesscontrolitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessLevel|Enumeration|This indicates an access level for the privacy data category to which the specified application will be given to. Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.|
|appDisplayName|String|The Package Family Name of a Windows app. When set, the access level applies to the specified application.|
|appPackageFamilyName|String|The Package Family Name of a Windows app. When set, the access level applies to the specified application.|
|dataCategory|Enumeration|This indicates a privacy data category to which the specific access control will apply. Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPrivacyDataAccessControlItem",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "String (identifier)",
  "accessLevel": "String",
  "dataCategory": "String",
  "appPackageFamilyName": "String",
  "appDisplayName": "String"
}
```

