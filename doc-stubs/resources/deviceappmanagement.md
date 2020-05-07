---
title: "deviceAppManagement resource type"
description: "Singleton entity that acts as a container for all device app management functionality."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceAppManagement resource type


Namespace: microsoft.graph

Singleton entity that acts as a container for all device app management functionality.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get deviceAppManagement](../api/deviceappmanagement-get.md)|[deviceAppManagement](../resources/deviceappmanagement.md)|Read the properties and relationships of a [deviceAppManagement](../resources/deviceappmanagement.md) object.|
|[Update deviceAppManagement](../api/deviceappmanagement-update.md)|[deviceAppManagement](../resources/deviceappmanagement.md)|Update the properties of a [deviceAppManagement](../resources/deviceappmanagement.md) object.|
|[List windowsManagementApp](../api/deviceappmanagement-list-windowsmanagementapp.md)|[windowsManagementApp](../resources/windowsmanagementapp.md) collection|Get the windowsManagementApps from the windowsManagementApp navigation property.|
|[Add windowsManagementApp](../api/deviceappmanagement-post-windowsmanagementapp.md)|[windowsManagementApp](../resources/windowsmanagementapp.md)|Add windowsManagementApp by posting to the windowsManagementApp collection.|
|[Remove windowsManagementApp](../api/deviceappmanagement-delete-windowsmanagementapp.md)|None|Remove a [windowsManagementApp](../resources/windowsmanagementapp.md) object.|
|[List windowsManagementApp2](../api/deviceappmanagement-list-windowsmanagementapp2.md)|[windowsManagementApp](../resources/windowsmanagementapp.md) collection|Get the windowsManagementApps from the windowsManagementApp2 navigation property.|
|[Add windowsManagementApp2](../api/deviceappmanagement-post-windowsmanagementapp2.md)|[windowsManagementApp](../resources/windowsmanagementapp.md)|Add windowsManagementApp2 by posting to the windowsManagementApp2 collection.|
|[Remove windowsManagementApp2](../api/deviceappmanagement-delete-windowsmanagementapp2.md)|None|Remove a [windowsManagementApp](../resources/windowsmanagementapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the entity.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|windowsManagementApp|[windowsManagementApp](../resources/windowsmanagementapp.md)|Windows management app.|
|windowsManagementApp2|[windowsManagementApp](../resources/windowsmanagementapp.md)|Windows management app.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.deviceAppManagement",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.deviceAppManagement",
  "id": "String (identifier)"
}
```

