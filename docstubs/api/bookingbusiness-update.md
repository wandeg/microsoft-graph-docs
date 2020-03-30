---
title: "Update bookingBusiness"
description: "Update the properties of a bookingBusiness object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update bookingBusiness

Namespace: microsoft.graph

Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.

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
PATCH /bookingBusinesses/{bookingBusinessesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [bookingBusiness](../resources/bookingbusiness.md) object.

The following table shows the properties that are required when you create the [bookingBusiness](../resources/bookingbusiness.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|businessType|String||
|address|[physicalAddress](../resources/physicaladdress.md)||
|phone|String||
|email|String||
|webSiteUrl|String||
|defaultCurrencyIso|String||
|businessHours|[bookingWorkHours](../resources/bookingworkhours.md) collection||
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)||
|isPublished|Boolean||
|publicUrl|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [bookingBusiness](../resources/bookingbusiness.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_bookingbusiness"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}
Content-type: application/json
Content-length: 1309

{
  "@odata.type": "#microsoft.graph.bookingBusiness",
  "displayName": "Display Name value",
  "businessType": "Business Type value",
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
  "phone": "Phone value",
  "email": "Email value",
  "webSiteUrl": "https://example.com/webSiteUrl/",
  "defaultCurrencyIso": "Default Currency Iso value",
  "businessHours": [
    {
      "@odata.type": "microsoft.graph.bookingWorkHours",
      "day": "String",
      "timeSlots": [
        {
          "@odata.type": "microsoft.graph.bookingWorkTimeSlot",
          "start": "11:56:38.3540000",
          "end": "12:02:04.8450000"
        }
      ]
    }
  ],
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
    "timeSlotInterval": "PT1M58.7102966S",
    "minimumLeadTime": "PT1M8.6653869S",
    "maximumAdvance": "PT45.2150091S",
    "sendConfirmationsToOwner": true,
    "allowStaffSelection": true
  },
  "isPublished": true,
  "publicUrl": "https://example.com/publicUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1358

{
  "@odata.type": "#microsoft.graph.bookingBusiness",
  "id": "7c4f0887-0887-7c4f-8708-4f7c87084f7c",
  "displayName": "Display Name value",
  "businessType": "Business Type value",
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
  "phone": "Phone value",
  "email": "Email value",
  "webSiteUrl": "https://example.com/webSiteUrl/",
  "defaultCurrencyIso": "Default Currency Iso value",
  "businessHours": [
    {
      "@odata.type": "microsoft.graph.bookingWorkHours",
      "day": "String",
      "timeSlots": [
        {
          "@odata.type": "microsoft.graph.bookingWorkTimeSlot",
          "start": "11:56:38.3540000",
          "end": "12:02:04.8450000"
        }
      ]
    }
  ],
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
    "timeSlotInterval": "PT1M58.7102966S",
    "minimumLeadTime": "PT1M8.6653869S",
    "maximumAdvance": "PT45.2150091S",
    "sendConfirmationsToOwner": true,
    "allowStaffSelection": true
  },
  "isPublished": true,
  "publicUrl": "https://example.com/publicUrl/"
}
```

