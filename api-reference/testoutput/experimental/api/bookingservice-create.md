---
title: "Create bookingService"
description: "Create a new bookingService object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create bookingService

Namespace: microsoft.graph

Create a new [bookingService](../resources/bookingservice.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /bookingBusinesses/{bookingBusinessesId}/services
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [bookingService](../resources/bookingservice.md) object.

The following table shows the properties that are required when you create the [bookingService](../resources/bookingservice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|defaultDuration|Duration||
|defaultLocation|[location](../resources/location.md)||
|defaultPrice|Double||
|defaultPriceType|Enumeration|. Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|defaultReminders|[bookingReminder](../resources/bookingreminder.md) collection|The default reminders set in an appointment of this service.
The value of this property is only available when reading an individual booking service by id.|
|description|String||
|isHiddenFromCustomers|Boolean||
|notes|String||
|preBuffer|Duration||
|postBuffer|Duration||
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)||
|staffMemberIds|String collection||



## Response
If successful, this method returns a `201 Created` response code and a [bookingService](../resources/bookingservice.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_bookingservice_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/bookingBusinesses/{bookingBusinessesId}/services
Content-type: application/json
Content-length: 1788

{
  "@odata.type": "#microsoft.graph.bookingService",
  "displayName": "Display Name value",
  "defaultDuration": "PT2M30.8894523S",
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
      "offset": "-PT2M15.3589096S",
      "recipients": "String",
      "message": "Message value"
    }
  ],
  "description": "Description value",
  "isHiddenFromCustomers": true,
  "notes": "Notes value",
  "preBuffer": "-PT27.6468082S",
  "postBuffer": "-PT49.745402S",
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
    "timeSlotInterval": "PT24.7084489S",
    "minimumLeadTime": "PT46.1171008S",
    "maximumAdvance": "-PT29.5884928S",
    "sendConfirmationsToOwner": true,
    "allowStaffSelection": true
  },
  "staffMemberIds": [
    "Staff Member Ids value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingservice"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1837

{
  "@odata.type": "#microsoft.graph.bookingService",
  "id": "dcfd9872-9872-dcfd-7298-fddc7298fddc",
  "displayName": "Display Name value",
  "defaultDuration": "PT2M30.8894523S",
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
      "offset": "-PT2M15.3589096S",
      "recipients": "String",
      "message": "Message value"
    }
  ],
  "description": "Description value",
  "isHiddenFromCustomers": true,
  "notes": "Notes value",
  "preBuffer": "-PT27.6468082S",
  "postBuffer": "-PT49.745402S",
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
    "timeSlotInterval": "PT24.7084489S",
    "minimumLeadTime": "PT46.1171008S",
    "maximumAdvance": "-PT29.5884928S",
    "sendConfirmationsToOwner": true,
    "allowStaffSelection": true
  },
  "staffMemberIds": [
    "Staff Member Ids value"
  ]
}
```

