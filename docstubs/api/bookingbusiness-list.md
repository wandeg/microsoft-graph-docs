---
title: "List bookingBusinesses"
description: "List properties and relationships of the bookingBusiness objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List bookingBusinesses

Namespace: microsoft.graph

List properties and relationships of the [bookingBusiness](../resources/bookingbusiness.md) objects.

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
GET /bookingBusinesses
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
If successful, this method returns a `200 OK` response code and a collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}
-->
``` http
GET https://graph.microsoft.com/beta/bookingBusinesses
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.bookingbusiness)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1556

{
  "value": [
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
  ]
}
```

