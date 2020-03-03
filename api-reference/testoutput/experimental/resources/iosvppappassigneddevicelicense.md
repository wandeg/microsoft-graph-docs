---
title: "iosVppAppAssignedDeviceLicense resource type"
description: "iOS Volume Purchase Program device license assignment. This class does not support Create, Delete, or Update."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosVppAppAssignedDeviceLicense resource type


Namespace: microsoft.graph

iOS Volume Purchase Program device license assignment. This class does not support Create, Delete, or Update.


Inherits from [iosVppAppAssignedLicense](../resources/iosvppappassignedlicense.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosVppAppAssignedDeviceLicenses](../api/iosvppappassigneddevicelicense-list.md)|[iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md) collection|List properties and relationships of the [iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md) objects.|
|[Get iosVppAppAssignedDeviceLicense](../api/iosvppappassigneddevicelicense-get.md)|[iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md)|Read properties and relationships of the [iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md) object.|
|[Create iosVppAppAssignedDeviceLicense](../api/iosvppappassigneddevicelicense-create.md)|[iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md)|Create a new [iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md) object.|
|[Delete iosVppAppAssignedDeviceLicense](../api/iosvppappassigneddevicelicense-delete.md)|None|Deletes a [iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md).|
|[Update iosVppAppAssignedDeviceLicense](../api/iosvppappassigneddevicelicense-update.md)|[iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md)|Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/iosvppappassigneddevicelicense.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceName|String|The device name.|
|id|String| Inherited from [entity](../resources/entity.md)|
|managedDeviceId|String|The managed device ID.|
|userEmailAddress|String|The user email address. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|The user ID. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|String|The user name. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|String|The user principal name. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|

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

