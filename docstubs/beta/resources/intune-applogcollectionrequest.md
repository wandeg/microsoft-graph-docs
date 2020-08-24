---
title: "appLogCollectionRequest resource type"
description: "AppLogCollectionRequest Entity."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# appLogCollectionRequest resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

AppLogCollectionRequest Entity.

## Methods

| Method                                                                            | Return Type                                                             | Description                                                             |
| :-------------------------------------------------------------------------------- | :---------------------------------------------------------------------- | :---------------------------------------------------------------------- |
| [List appLogCollectionRequest](../api/intune-applogcollectionrequest-list.md)     | [appLogCollectionRequest](intune-appLogCollectionRequest.md) collection | List properties and relationships of an appLogCollectionRequest object. |
| [Create appLogCollectionRequest](../api/intune-applogcollectionrequest-create.md) | [appLogCollectionRequest](intune-appLogCollectionRequest.md)            | Create a new appLogCollectionRequest object.                            |
| [Get appLogCollectionRequest](../api/intune-applogcollectionrequest-get.md)       | [appLogCollectionRequest](intune-appLogCollectionRequest.md)            | Read properties and relationships of an appLogCollectionRequest object. |
| [Update appLogCollectionRequest](../api/intune-applogcollectionrequest-update.md) | [appLogCollectionRequest](intune-appLogCollectionRequest.md)            | Update the properties of an appLogCollectionRequest object.             |
| [Delete appLogCollectionRequest](../api/intune-applogcollectionrequest-delete.md) |                                                                         | Delete an appLogCollectionRequest object.                               |
| [createDownloadUrl](../api/intune-applogcollectionrequest-createDownloadUrl.md)   | appLogCollectionDownloadDetails                                         |                                                                         |

## Properties

| Property          | Type              | Description                                                         |
| :---------------- | :---------------- | :------------------------------------------------------------------ |
| completedDateTime | DateTimeOffset    | Time at which the upload log request reached a terminal state       |
| customLogFolders  | String collection | List of log folders.                                                |
| errorMessage      | String            | Error message if any during the upload process                      |
| id                | String            | The unique Identifier. This is userId_DeviceId_AppId id. Read-only. |
| status            | String            | Log upload status                                                   |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appLogCollectionRequest",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "completedDateTime": "DateTimeOffset",
  "customLogFolders": ["String"],
  "errorMessage": "String",
  "id": "String (identifier)",
  "status": "pending | completed | failed"
}
```