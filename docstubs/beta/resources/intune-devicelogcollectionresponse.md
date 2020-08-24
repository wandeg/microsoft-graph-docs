---
title: "deviceLogCollectionResponse resource type"
description: "Windows Log Collection request entity."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceLogCollectionResponse resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows Log Collection request entity.

## Methods

| Method                                                                                    | Return Type                                                                     | Description                                                                |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ | :------------------------------------------------------------------------- |
| [List deviceLogCollectionResponse](../api/intune-devicelogcollectionresponse-list.md)     | [deviceLogCollectionResponse](intune-deviceLogCollectionResponse.md) collection | List properties and relationships of a deviceLogCollectionResponse object. |
| [Create deviceLogCollectionResponse](../api/intune-devicelogcollectionresponse-create.md) | [deviceLogCollectionResponse](intune-deviceLogCollectionResponse.md)            | Create a new deviceLogCollectionResponse object.                           |
| [Get deviceLogCollectionResponse](../api/intune-devicelogcollectionresponse-get.md)       | [deviceLogCollectionResponse](intune-deviceLogCollectionResponse.md)            | Read properties and relationships of a deviceLogCollectionResponse object. |
| [Update deviceLogCollectionResponse](../api/intune-devicelogcollectionresponse-update.md) | [deviceLogCollectionResponse](intune-deviceLogCollectionResponse.md)            | Update the properties of a deviceLogCollectionResponse object.             |
| [Delete deviceLogCollectionResponse](../api/intune-devicelogcollectionresponse-delete.md) |                                                                                 | Delete a deviceLogCollectionResponse object.                               |
| [createDownloadUrl](../api/intune-devicelogcollectionresponse-createDownloadUrl.md)       | String                                                                          |                                                                            |

## Properties

| Property                     | Type           | Description                                                                        |
| :--------------------------- | :------------- | :--------------------------------------------------------------------------------- |
| errorCode                    | Int64          | The error code, if any. Valid values -9.22337203685478E+18 to 9.22337203685478E+18 |
| expirationDateTimeUTC        | DateTimeOffset | The DateTime of the expiration of the logs                                         |
| id                           | String         | The unique identifier in the form of tenantId_deviceId_requestId Read-only.        |
| initiatedByUserPrincipalName | String         | The UPN for who initiated the request                                              |
| managedDeviceId              | Guid           | The device Id                                                                      |
| receivedDateTimeUTC          | DateTimeOffset | The DateTime the request was received                                              |
| requestedDateTimeUTC         | DateTimeOffset | The DateTime of the request                                                        |
| size                         | Double         | The size of the logs. Valid values -1.79769313486232E+308 to 1.79769313486232E+308 |
| status                       | String         | The status of the log collection request                                           |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceLogCollectionResponse",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "errorCode": "Int64",
  "expirationDateTimeUTC": "DateTimeOffset",
  "id": "String (identifier)",
  "initiatedByUserPrincipalName": "String",
  "managedDeviceId": "Guid",
  "receivedDateTimeUTC": "DateTimeOffset",
  "requestedDateTimeUTC": "DateTimeOffset",
  "size": "Double",
  "status": "String"
}
```