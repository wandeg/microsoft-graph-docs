---
title: "mobileAppTroubleshootingEvent resource type"
description: "MobileAppTroubleshootingEvent Entity."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# mobileAppTroubleshootingEvent resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

MobileAppTroubleshootingEvent Entity.

## Methods

| Method                                                                                                     | Return Type                                                                  | Description                                                                           |
| :--------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------- | :------------------------------------------------------------------------------------ |
| [List mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-list.md)                         | [mobileAppTroubleshootingEvent](mobileAppTroubleshootingEvent.md) collection | List properties and relationships of a mobileAppTroubleshootingEvent object.          |
| [Create mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-create.md)                     | [mobileAppTroubleshootingEvent](mobileAppTroubleshootingEvent.md)            | Create a new mobileAppTroubleshootingEvent object.                                    |
| [Get mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-get.md)                           | [mobileAppTroubleshootingEvent](mobileAppTroubleshootingEvent.md)            | Read properties and relationships of a mobileAppTroubleshootingEvent object.          |
| [Update mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-update.md)                     | [mobileAppTroubleshootingEvent](mobileAppTroubleshootingEvent.md)            | Update the properties of a mobileAppTroubleshootingEvent object.                      |
| [Delete mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-delete.md)                     |                                                                              | Delete a mobileAppTroubleshootingEvent object.                                        |
| [List appLogCollectionRequests](../api/mobileapptroubleshootingevent-list-applogcollectionrequests.md)     | appLogCollectionRequest                                                      | Get the appLogCollectionRequest from an appLogCollectionRequests navigation property. |
| [Create appLogCollectionRequests](../api/mobileapptroubleshootingevent-post-applogcollectionrequests.md)   | appLogCollectionRequest                                                      | Create a new appLogCollectionRequests object.                                         |
| [Get appLogCollectionRequests](../api/mobileapptroubleshootingevent-get-applogcollectionrequests.md)       | appLogCollectionRequest                                                      | Read the properties and relationships of an appLogCollectionRequest object.           |
| [Update appLogCollectionRequests](../api/mobileapptroubleshootingevent-update-applogcollectionrequests.md) | appLogCollectionRequest                                                      | Update the properties of an appLogCollectionRequests object.                          |
| [Delete appLogCollectionRequests](../api/mobileapptroubleshootingevent-delete-applogcollectionrequests.md) |                                                                              | Delete an appLogCollectionRequest object.                                             |

## Properties

| Property | Type   | Description                        |
| :------- | :----- | :--------------------------------- |
| id       | String | The GUID for the object Read-only. |

## Relationships

| Relationship             | Type                                                                          | Description                                     |
| :----------------------- | :---------------------------------------------------------------------------- | :---------------------------------------------- |
| appLogCollectionRequests | [appLogCollectionRequest](../resources/applogcollectionrequest.md) collection | The collection property of AppLogUploadRequest. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "String (identifier)"
}
```