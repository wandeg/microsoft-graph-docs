---
title: "Create services"
description: "Create a new services object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create services

Namespace: microsoft.graph

Create a new services object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /bookingBusinesses/{bookingBusinessesId}/services
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [bookingService](../resources/bookingservice.md) object.

The following table shows the properties that are required when you create the [bookingService](../resources/bookingservice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|defaultDuration|Duration|**TODO: Add Description**|
|defaultLocation|[location](../resources/location.md)|**TODO: Add Description**|
|defaultPrice|Double|**TODO: Add Description**|
|defaultPriceType|bookingPriceType|**TODO: Add Description**. Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|defaultReminders|[bookingReminder](../resources/bookingreminder.md) collection|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|isHiddenFromCustomers|Boolean|**TODO: Add Description**|
|notes|String|**TODO: Add Description**|
|preBuffer|Duration|**TODO: Add Description**|
|postBuffer|Duration|**TODO: Add Description**|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|**TODO: Add Description**|
|staffMemberIds|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [bookingService](../resources/bookingservice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_bookingservice_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/services
Content-Type: application/json
Content-length: 667

{
  "@odata.type": "#microsoft.graph.bookingService",
  "displayName": "String",
  "defaultDuration": "String (duration)",
  "defaultLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "defaultPrice": "Double",
  "defaultPriceType": "String",
  "defaultReminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder"
    }
  ],
  "description": "String",
  "isHiddenFromCustomers": "Boolean",
  "notes": "String",
  "preBuffer": "String (duration)",
  "postBuffer": "String (duration)",
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
  },
  "staffMemberIds": [
    "String"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingservice"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.bookingService",
  "id": "67351234-1234-6735-3412-356734123567",
  "displayName": "String",
  "defaultDuration": "String (duration)",
  "defaultLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "defaultPrice": "Double",
  "defaultPriceType": "String",
  "defaultReminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder"
    }
  ],
  "description": "String",
  "isHiddenFromCustomers": "Boolean",
  "notes": "String",
  "preBuffer": "String (duration)",
  "postBuffer": "String (duration)",
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
  },
  "staffMemberIds": [
    "String"
  ]
}
```

