---
title: "Update bookingBusiness"
description: "Update the properties of a bookingBusiness object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update bookingBusiness

Namespace: microsoft.graph

Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.

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
PATCH /bookingBusinesses/{bookingBusinessesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [bookingBusiness](../resources/bookingbusiness.md) object.

The following table shows the properties that are required when you create the [bookingBusiness](../resources/bookingbusiness.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|businessType|String|**TODO: Add Description**|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|phone|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|webSiteUrl|String|The URL of the business web site.
Example: https://www.contoso.com|
|defaultCurrencyIso|String|**TODO: Add Description**|
|businessHours|[bookingWorkHours](../resources/bookingworkhours.md) collection|**TODO: Add Description**|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|**TODO: Add Description**|
|isPublished|Boolean|**TODO: Add Description**|
|publicUrl|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [bookingBusiness](../resources/bookingbusiness.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_bookingbusiness"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}
Content-Type: application/json
Content-length: 1311

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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

