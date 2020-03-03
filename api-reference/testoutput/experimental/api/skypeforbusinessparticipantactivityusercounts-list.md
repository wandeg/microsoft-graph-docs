---
title: "List skypeForBusinessParticipantActivityUserCountses"
description: "List properties and relationships of the skypeForBusinessParticipantActivityUserCounts objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List skypeForBusinessParticipantActivityUserCountses

Namespace: microsoft.graph

List properties and relationships of the [skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md) objects.

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
GET ** Collection URI for microsoft.graph.skypeForBusinessParticipantActivityUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_skypeforbusinessparticipantactivityusercounts"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.skypeForBusinessParticipantActivityUserCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.skypeforbusinessparticipantactivityusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 402

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.skypeForBusinessParticipantActivityUserCounts",
      "id": "840cb8ca-b8ca-840c-cab8-0c84cab80c84",
      "im": 2,
      "audioVideo": 10,
      "appSharing": 10,
      "web": 3,
      "dialInOut3rdParty": 1,
      "reportRefreshDate": "Date",
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

