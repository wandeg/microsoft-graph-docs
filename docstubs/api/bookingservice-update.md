---
title: "Update bookingService"
description: "Update the properties of a bookingService object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update bookingService

Namespace: microsoft.graph

Update the properties of a [bookingService](../resources/bookingservice.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /bookingBusinesses/{bookingBusinessesId}/services/{bookingServiceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [bookingService](../resources/bookingservice.md) object.

The following table shows the properties that are required when you create the [bookingService](../resources/bookingservice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|defaultDuration|Duration||
|defaultLocation|[location](../resources/location.md)||
|defaultPrice|Double||
|defaultPriceType|Enumeration| Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|defaultReminders|[bookingReminder](../resources/bookingreminder.md) collection||
|description|String||
|isHiddenFromCustomers|Boolean||
|notes|String||
|preBuffer|Duration||
|postBuffer|Duration||
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)||
|staffMemberIds|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [bookingService](../resources/bookingservice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/services/{bookingServiceId}
Content-type: application/json
Content-length: 1791

{
  "@odata.type": "#microsoft.graph.bookingService",
  "displayName": "Display Name value",
  "defaultDuration": "PT32.7563926S",
  "defaultLocation": {
    "@odata.type": "microsoft.graph.location",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "type": "String",
      "postOfficeBox": "Post Office Box value",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationUri": "Location Uri value",
    "locationType": "String",
    "uniqueId": "Unique Id value",
    "uniqueIdType": "String"
  },
  "defaultPrice": "Double",
  "defaultPriceType": "String",
  "defaultReminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder",
      "offset": "PT3.2720379S",
      "recipients": "String",
      "message": "Message value"
    }
  ],
  "description": "Description value",
  "isHiddenFromCustomers": true,
  "notes": "Notes value",
  "preBuffer": "PT1M54.2429074S",
  "postBuffer": "-PT2M56.6678405S",
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
    "timeSlotInterval": "-PT1M10.9790526S",
    "minimumLeadTime": "PT1M25.106348S",
    "maximumAdvance": "PT1M14.5055198S",
    "sendConfirmationsToOwner": true,
    "allowStaffSelection": true
  },
  "staffMemberIds": [
    "Staff Member Ids value"
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1840

{
  "@odata.type": "#microsoft.graph.bookingService",
  "id": "0652ebb2-ebb2-0652-b2eb-5206b2eb5206",
  "displayName": "Display Name value",
  "defaultDuration": "PT32.7563926S",
  "defaultLocation": {
    "@odata.type": "microsoft.graph.location",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "type": "String",
      "postOfficeBox": "Post Office Box value",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationUri": "Location Uri value",
    "locationType": "String",
    "uniqueId": "Unique Id value",
    "uniqueIdType": "String"
  },
  "defaultPrice": "Double",
  "defaultPriceType": "String",
  "defaultReminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder",
      "offset": "PT3.2720379S",
      "recipients": "String",
      "message": "Message value"
    }
  ],
  "description": "Description value",
  "isHiddenFromCustomers": true,
  "notes": "Notes value",
  "preBuffer": "PT1M54.2429074S",
  "postBuffer": "-PT2M56.6678405S",
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
    "timeSlotInterval": "-PT1M10.9790526S",
    "minimumLeadTime": "PT1M25.106348S",
    "maximumAdvance": "PT1M14.5055198S",
    "sendConfirmationsToOwner": true,
    "allowStaffSelection": true
  },
  "staffMemberIds": [
    "Staff Member Ids value"
  ]
}
```

