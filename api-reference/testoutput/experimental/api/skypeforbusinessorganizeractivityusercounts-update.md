---
title: "Update skypeForBusinessOrganizerActivityUserCounts"
description: "Update the properties of a skypeForBusinessOrganizerActivityUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update skypeForBusinessOrganizerActivityUserCounts

Namespace: microsoft.graph

Update the properties of a [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.skypeForBusinessOrganizerActivityUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) object.

The following table shows the properties that are required when you create the [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|im|Int64||
|audioVideo|Int64||
|appSharing|Int64||
|web|Int64||
|dialInOut3rdParty|Int64||
|dialInOutMicrosoft|Int64||
|reportRefreshDate|Date||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_skypeforbusinessorganizeractivityusercounts"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.skypeForBusinessOrganizerActivityUserCounts not found
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.skypeForBusinessOrganizerActivityUserCounts",
  "im": 2,
  "audioVideo": 10,
  "appSharing": 10,
  "web": 3,
  "dialInOut3rdParty": 1,
  "dialInOutMicrosoft": 2,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
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
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.skypeForBusinessOrganizerActivityUserCounts",
  "id": "d1872f26-2f26-d187-262f-87d1262f87d1",
  "im": 2,
  "audioVideo": 10,
  "appSharing": 10,
  "web": 3,
  "dialInOut3rdParty": 1,
  "dialInOutMicrosoft": 2,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

