---
title: "Create bookingBusiness"
description: "Create a new bookingBusiness object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create bookingBusiness

Namespace: microsoft.graph

Create a new [bookingBusiness](../resources/bookingbusiness.md) object.

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
POST /bookingBusinesses
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [bookingBusiness](../resources/bookingbusiness.md) object.

The following table shows the properties that are required when you create the [bookingBusiness](../resources/bookingbusiness.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|businessType|String|**TODO: Add Description**|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|phone|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|webSiteUrl|String|**TODO: Add Description**|
|defaultCurrencyIso|String|**TODO: Add Description**|
|businessHours|[bookingWorkHours](../resources/bookingworkhours.md) collection|**TODO: Add Description**|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|**TODO: Add Description**|
|isPublished|Boolean|**TODO: Add Description**|
|publicUrl|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [bookingBusiness](../resources/bookingbusiness.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_bookingbusiness_from_bookingbusinesses"
}
-->
``` http
POST https://graph.microsoft.com/beta/bookingBusinesses
Content-Type: application/json
Content-length: 543

{
  "@odata.type": "#microsoft.graph.bookingBusiness",
  "displayName": "String",
  "businessType": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "phone": "String",
  "email": "String",
  "webSiteUrl": "String",
  "defaultCurrencyIso": "String",
  "businessHours": [
    {
      "@odata.type": "microsoft.graph.bookingWorkHours"
    }
  ],
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
  },
  "isPublished": "Boolean",
  "publicUrl": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingbusiness"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.bookingBusiness",
  "id": "99b37047-7047-99b3-4770-b3994770b399",
  "displayName": "String",
  "businessType": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "phone": "String",
  "email": "String",
  "webSiteUrl": "String",
  "defaultCurrencyIso": "String",
  "businessHours": [
    {
      "@odata.type": "microsoft.graph.bookingWorkHours"
    }
  ],
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
  },
  "isPublished": "Boolean",
  "publicUrl": "String"
}
```

