---
title: "Create bookingBusiness"
description: "Create a new bookingBusiness object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create bookingBusiness

Namespace: microsoft.graph

Create a new [bookingBusiness](../resources/bookingbusiness.md) object.

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
POST /bookingBusinesses
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [bookingBusiness](../resources/bookingbusiness.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_bookingbusiness_from_bookingbusinesses"
}
-->
``` http
POST https://graph.microsoft.com/beta/bookingBusinesses
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
          "start": "12:03:10.1400000",
          "end": "12:01:43.5200000"
        }
      ]
    }
  ],
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
    "timeSlotInterval": "PT2M16.0090163S",
    "minimumLeadTime": "PT16.0566243S",
    "maximumAdvance": "PT2M12.9589577S",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingbusiness"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1359

{
  "@odata.type": "#microsoft.graph.bookingBusiness",
  "id": "9d235d79-5d79-9d23-795d-239d795d239d",
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
          "start": "12:03:10.1400000",
          "end": "12:01:43.5200000"
        }
      ]
    }
  ],
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
    "timeSlotInterval": "PT2M16.0090163S",
    "minimumLeadTime": "PT16.0566243S",
    "maximumAdvance": "PT2M12.9589577S",
    "sendConfirmationsToOwner": true,
    "allowStaffSelection": true
  },
  "isPublished": true,
  "publicUrl": "https://example.com/publicUrl/"
}
```

