---
title: "dataSharingConsent resource type"
description: "Data sharing consent information."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# dataSharingConsent resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Data sharing consent information.

## Methods

| Method                                                                           | Return Type                                                   | Description                                                       |
| :------------------------------------------------------------------------------- | :------------------------------------------------------------ | :---------------------------------------------------------------- |
| [List dataSharingConsent](../api/intune-datasharingconsent-list.md)              | [dataSharingConsent](intune-dataSharingConsent.md) collection | List properties and relationships of a dataSharingConsent object. |
| [Create dataSharingConsent](../api/intune-datasharingconsent-create.md)          | [dataSharingConsent](intune-dataSharingConsent.md)            | Create a new dataSharingConsent object.                           |
| [Get dataSharingConsent](../api/intune-datasharingconsent-get.md)                | [dataSharingConsent](intune-dataSharingConsent.md)            | Read properties and relationships of a dataSharingConsent object. |
| [Update dataSharingConsent](../api/intune-datasharingconsent-update.md)          | [dataSharingConsent](intune-dataSharingConsent.md)            | Update the properties of a dataSharingConsent object.             |
| [Delete dataSharingConsent](../api/intune-datasharingconsent-delete.md)          |                                                               | Delete a dataSharingConsent object.                               |
| [consentToDataSharing](../api/intune-datasharingconsent-consentToDataSharing.md) | dataSharingConsent                                            |                                                                   |

## Properties

| Property           | Type           | Description                                                  |
| :----------------- | :------------- | :----------------------------------------------------------- |
| grantDateTime      | DateTimeOffset | The time consent was granted for this account                |
| granted            | Boolean        | The granted state for the data sharing consent               |
| grantedByUpn       | String         | The Upn of the user that granted consent for this account    |
| grantedByUserId    | String         | The UserId of the user that granted consent for this account |
| id                 | String         | The data sharing consent Id Read-only.                       |
| serviceDisplayName | String         | The display name of the service work flow                    |
| termsUrl           | String         | The TermsUrl for the data sharing consent                    |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "grantDateTime": "DateTimeOffset",
  "granted": "Boolean",
  "grantedByUpn": "String",
  "grantedByUserId": "String",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String"
}
```