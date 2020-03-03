---
title: "iosVppAppAssignedDeviceLicense resource type"
description: "iOS Volume Purchase Program device license assignment. This class does not support Create, Delete, or Update."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# iosVppAppAssignedDeviceLicense resource type

iOS Volume Purchase Program device license assignment. This class does not support Create, Delete, or Update.


Inherits from [iosVppAppAssignedLicense](../resources/iosVppAppAssignedLicense.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosVppAppAssignedDeviceLicenses](../api/iosvppappassigneddevicelicense-list.md)|[iosVppAppAssignedDeviceLicense](../resources/iosVppAppAssignedDeviceLicense.md) collection|List properties and relationships of the [iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md) objects.|
|[Get iosVppAppAssignedDeviceLicense](../api/iosvppappassigneddevicelicense-get.md)|[iosVppAppAssignedDeviceLicense](../resources/iosVppAppAssignedDeviceLicense.md)|Read properties and relationships of the [iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md) object.|
|[Create iosVppAppAssignedDeviceLicense](../api/iosvppappassigneddevicelicense-create.md)|[iosVppAppAssignedDeviceLicense](../resources/iosVppAppAssignedDeviceLicense.md)|Create a new [iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md) object.|
|[Delete iosVppAppAssignedDeviceLicense](../api/iosvppappassigneddevicelicense-delete.md)|None|Deletes a [iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md).|
|[Update iosVppAppAssignedDeviceLicense](../api/iosvppappassigneddevicelicense-update.md)|[iosVppAppAssignedDeviceLicense](../resources/iosVppAppAssignedDeviceLicense.md)|Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceName|String|The device name.|
|id|String| Inherited from [entity](../resources/entity.md)|
|managedDeviceId|String|The managed device ID.|
|userEmailAddress|String|The user email address. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosVppAppAssignedLicense.md)|
|userId|String|The user ID. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosVppAppAssignedLicense.md)|
|userName|String|The user name. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosVppAppAssignedLicense.md)|
|userPrincipalName|String|The user principal name. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosVppAppAssignedLicense.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedDeviceLicense",
  "baseType": "microsoft.graph.iosVppAppAssignedLicense",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "managedDeviceId": "String",
  "deviceName": "String"
}
```

