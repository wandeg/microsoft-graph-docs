---
title: "applePushNotificationCertificate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# applePushNotificationCertificate resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List applePushNotificationCertificate](../api/intune-devicemanagement-list-applepushnotificationcertificate.md)|[applePushNotificationCertificate](../resources/intune-applepushnotificationcertificate.md) collection|Get the applePushNotificationCertificates from the applePushNotificationCertificate navigation property.|
|[Create applePushNotificationCertificate](../api/intune-devicemanagement-post-applepushnotificationcertificate.md)|[applePushNotificationCertificate](../resources/intune-applepushnotificationcertificate.md)|Create a new applePushNotificationCertificate object.|
|[Delete applePushNotificationCertificate](../api/intune-devicemanagement-delete-applepushnotificationcertificate.md)|None|Delete an [applePushNotificationCertificate](../resources/intune-applepushnotificationcertificate.md) object.|
|[Update applePushNotificationCertificate](../api/intune-devicemanagement-update-applepushnotificationcertificate.md)|[applePushNotificationCertificate](../resources/intune-applepushnotificationcertificate.md)|Update the properties of an applePushNotificationCertificate object.|
|[Get applePushNotificationCertificate](../api/intune-devicemanagement-get-applepushnotificationcertificate.md)|[applePushNotificationCertificate](../resources/intune-applepushnotificationcertificate.md)|Read the properties and relationships of an [applePushNotificationCertificate](../resources/intune-applepushnotificationcertificate.md) object.|
|[downloadApplePushNotificationCertificateSigningRequest](../api/intune-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|String|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleIdentifier|String|**TODO: Add Description**|
|certificate|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|topicIdentifier|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```

