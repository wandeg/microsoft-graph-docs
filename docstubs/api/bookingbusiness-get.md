---
title: "Get bookingBusiness"
description: "Read properties and relationships of the bookingBusiness object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get bookingBusiness

Namespace: microsoft.graph

Read properties and relationships of the [bookingBusiness](../resources/bookingbusiness.md) object.

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
GET /bookingBusinesses/{bookingBusinessesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}
-->
``` http
GET https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1462

{
  "value": {
    "@odata.type": "#microsoft.graph.bookingBusiness",
    "id": "526ba279-a279-526b-79a2-6b5279a26b52",
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
            "start": "11:56:56.0110000",
            "end": "11:57:00.7790000"
          }
        ]
      }
    ],
    "schedulingPolicy": {
      "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
      "timeSlotInterval": "-PT1M10.9790526S",
      "minimumLeadTime": "PT1M25.106348S",
      "maximumAdvance": "PT1M14.5055198S",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
    },
    "isPublished": true,
    "publicUrl": "https://example.com/publicUrl/"
  }
}
```

