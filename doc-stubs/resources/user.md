---
title: "user resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# user resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List users](../api/user-list.md)|[user](../resources/user.md) collection|Get a list of the [user](../resources/user.md) objects and their properties.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read the properties and relationships of a [user](../resources/user.md) object.|
|[Create user](../api/user-post-users.md)|[user](../resources/user.md)|Create a new [user](../resources/user.md) object.|
|[Delete user](../api/user-delete.md)|None|Deletes a [user](../resources/user.md) object.|
|[Update user](../api/user-update.md)|[user](../resources/user.md)|Update the properties of a [user](../resources/user.md) object.|
|[removeAllDevicesFromManagement](../api/user-removealldevicesfrommanagement.md)|None|Retire all devices from management for this user|
|[getLoggedOnManagedDevices](../api/user-getloggedonmanageddevices.md)|[managedDevice](../resources/manageddevice.md) collection|**TODO: Add Description**|
|[getLoggedOnManagedDevices2](../api/user-getloggedonmanageddevices2.md)|[managedDevice](../resources/manageddevice.md) collection|**TODO: Add Description**|
|[List managedDevices](../api/user-list-manageddevices.md)|[managedDevice](../resources/manageddevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Create managedDevices](../api/user-post-manageddevices.md)|[managedDevice](../resources/manageddevice.md)|Create a new managedDevices object.|
|[Delete managedDevices](../api/user-delete-manageddevices.md)|None|Delete a [managedDevice](../resources/manageddevice.md) object.|
|[Update managedDevices](../api/user-update-manageddevices.md)|[managedDevice](../resources/manageddevice.md)|Update the properties of a managedDevices object.|
|[Get managedDevice](../api/manageddevice-get.md)|[managedDevice](../resources/manageddevice.md)|Read the properties and relationships of a [managedDevice](../resources/manageddevice.md) object.|
|[List managedDevices2](../api/user-list-manageddevices2.md)|[managedDevice](../resources/manageddevice.md) collection|Get the managedDevices from the managedDevices2 navigation property.|
|[Create managedDevices2](../api/user-post-manageddevices2.md)|[managedDevice](../resources/manageddevice.md)|Create a new managedDevices2 object.|
|[Delete managedDevices2](../api/user-delete-manageddevices2.md)|None|Delete a [managedDevice](../resources/manageddevice.md) object.|
|[Update managedDevices2](../api/user-update-manageddevices2.md)|[managedDevice](../resources/manageddevice.md)|Update the properties of a managedDevices2 object.|
|[Get managedDevice](../api/manageddevice-get.md)|[managedDevice](../resources/manageddevice.md)|Read the properties and relationships of a [managedDevice](../resources/manageddevice.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Unique identifier of the user.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managedDevices|[managedDevice](../resources/manageddevice.md) collection|The managed devices associated with the user.|
|managedDevices2|[managedDevice](../resources/manageddevice.md) collection|The managed devices associated with the user.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.user",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.user",
  "id": "String (identifier)"
}
```

