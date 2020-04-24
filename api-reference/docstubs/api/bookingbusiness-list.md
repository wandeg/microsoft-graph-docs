---
title: "List bookingBusinesses"
description: "Get a list of the bookingBusiness objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List bookingBusinesses

Namespace: microsoft.graph

Get a list of the [bookingBusiness](../resources/bookingbusiness.md) objects and their properties.

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
GET /bookingBusinesses
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}
-->
``` http
GET https://graph.microsoft.com/beta/bookingBusinesses
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.bookingbusiness)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bookingBusiness",
      "id": "36837c0d-7c0d-3683-0d7c-83360d7c8336",
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
              "start": "12:02:33.8790000",
              "end": "12:02:09.0100000"
            }
          ]
        }
      ],
      "schedulingPolicy": {
        "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
        "timeSlotInterval": "-PT54.217212S",
        "minimumLeadTime": "PT2M50.4712447S",
        "maximumAdvance": "-PT2M45.2265401S",
        "sendConfirmationsToOwner": true,
        "allowStaffSelection": true
      },
      "isPublished": true,
      "publicUrl": "https://example.com/publicUrl/"
    }
  ]
}
```

