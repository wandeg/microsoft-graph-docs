---
title: "deviceManagementPartner resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementPartner resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementPartner](../api/devicemanagementpartner-get.md)|[deviceManagementPartner](../resources/devicemanagementpartner.md)|Read properties and relationships of the [deviceManagementPartner](../resources/devicemanagementpartner.md) object.|
|[Update deviceManagementPartner](../api/devicemanagementpartner-update.md)|[deviceManagementPartner](../resources/devicemanagementpartner.md)|Update the properties of a [deviceManagementPartner](../resources/devicemanagementpartner.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|groupsRequiringPartnerEnrollment|[deviceManagementPartnerAssignment](../resources/devicemanagementpartnerassignment.md) collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|isConfigured|Boolean||
|lastHeartbeatDateTime|DateTimeOffset||
|partnerAppType|Enumeration| Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.|
|partnerState|Enumeration| Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|singleTenantAppId|String||
|whenPartnerDevicesWillBeMarkedAsNonCompliant|DateTimeOffset||
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset||
|whenPartnerDevicesWillBeRemoved|DateTimeOffset||
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "String (timestamp)",
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
    }
  ]
}
```

