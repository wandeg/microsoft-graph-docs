---
title: "subscription resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# subscription resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get subscription](../api/subscription-get.md)|[subscription](../resources/subscription.md)|Read properties and relationships of the [subscription](../resources/subscription.md) object.|
|[Delete subscription](../api/subscription-delete.md)|None|Deletes a [subscription](../resources/subscription.md).|
|[Update subscription](../api/subscription-update.md)|[subscription](../resources/subscription.md)|Update the properties of a [subscription](../resources/subscription.md) object.|
|[List subscriptions](../api/driveitem-list-subscriptions.md)|[subscription](../resources/subscription.md) collection|Get the subscriptions from the subscriptions navigation property.|
|[Add subscriptions](../api/driveitem-post-subscriptions.md)|[subscription](../resources/subscription.md)|Add subscriptions by posting to the subscriptions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationId|String||
|changeType|String||
|clientState|String||
|creatorId|String||
|encryptionCertificate|String||
|encryptionCertificateId|String||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|includeProperties|Boolean||
|includeResourceData|Boolean||
|lifecycleNotificationUrl|String||
|notificationUrl|String||
|resource|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscription",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subscription",
  "id": "String (identifier)",
  "resource": "String",
  "changeType": "String",
  "clientState": "String",
  "notificationUrl": "String",
  "expirationDateTime": "String (timestamp)",
  "applicationId": "String",
  "creatorId": "String",
  "includeProperties": true,
  "includeResourceData": true,
  "lifecycleNotificationUrl": "String",
  "encryptionCertificate": "String",
  "encryptionCertificateId": "String"
}
```

