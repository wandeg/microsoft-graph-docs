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
Content-length: 1310

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
          "start": "11:58:13.3440000",
          "end": "12:01:29.0340000"
        }
      ]
    }
  ],
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
    "timeSlotInterval": "-PT2M34.907001S",
    "minimumLeadTime": "-PT3M17.4420665S",
    "maximumAdvance": "PT7.3457796S",
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
Content-Length: 1359

{
  "@odata.type": "#microsoft.graph.bookingBusiness",
  "id": "5851a833-a833-5851-33a8-515833a85158",
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
          "start": "11:58:13.3440000",
          "end": "12:01:29.0340000"
        }
      ]
    }
  ],
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
    "timeSlotInterval": "-PT2M34.907001S",
    "minimumLeadTime": "-PT3M17.4420665S",
    "maximumAdvance": "PT7.3457796S",
    "sendConfirmationsToOwner": true,
    "allowStaffSelection": true
  },
  "isPublished": true,
  "publicUrl": "https://example.com/publicUrl/"
}
```

