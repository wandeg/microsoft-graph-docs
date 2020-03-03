---
title: "List callRecords"
description: "List properties and relationships of the callRecord objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List callRecords

Namespace: microsoft.graph.callRecords

List properties and relationships of the [callRecord](../resources/callrecord.md) objects.

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
GET /communications/callRecords
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [callRecord](../resources/callrecord.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_callrecord"
}
-->
``` http
GET https://graph.microsoft.com/localtest/communications/callRecords
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.callrecords.callrecord)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1032

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.callRecords.callRecord",
      "id": "319f7649-7649-319f-4976-9f3149769f31",
      "version": 7,
      "type": "String",
      "modalities": [
        "String"
      ],
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
      "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
      "organizer": {
        "@odata.type": "microsoft.graph.identitySet",
        "application": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value",
          "displayName": "Display Name value"
        },
        "device": {
          "@odata.type": "microsoft.graph.identity"
        },
        "user": {
          "@odata.type": "microsoft.graph.identity"
        }
      },
      "participants": [
        {
          "@odata.type": "microsoft.graph.identitySet"
        }
      ],
      "joinWebUrl": "https://example.com/joinWebUrl/"
    }
  ]
}
```

