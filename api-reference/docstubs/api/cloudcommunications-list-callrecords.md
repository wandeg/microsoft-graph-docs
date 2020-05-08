---
title: "List callRecords"
description: "Get the callRecords from the callRecords navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List callRecords

Namespace: microsoft.graph.callRecords

Get the callRecords from the callRecords navigation property.

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
GET /communications/callRecords
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
If successful, this method returns a `200 OK` response code and a collection of [callRecord](../resources/callrecord.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_callrecord"
}
-->
``` http
GET https://graph.microsoft.com/beta/communications/callRecords
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.callrecords.callrecord)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.callRecords.callRecord",
      "version": 7,
      "type": "String",
      "modalities": [
        "String"
      ],
      "lastModifiedDateTime": "2016-12-31T23:57:20.9414035+03:00",
      "startDateTime": "2016-12-31T23:56:48.8437798+03:00",
      "endDateTime": "2016-12-31T23:57:13.0779697+03:00",
      "organizer": {
        "@odata.type": "microsoft.graph.identitySet",
        "user": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value",
          "displayName": "Display Name value"
        },
        "application": {
          "@odata.type": "microsoft.graph.identity"
        },
        "device": {
          "@odata.type": "microsoft.graph.identity"
        }
      },
      "participants": [
        {
          "@odata.type": "microsoft.graph.identitySet"
        }
      ],
      "joinWebUrl": "https://example.com/joinWebUrl/",
      "id": "8b02753b-753b-8b02-3b75-028b3b75028b"
    }
  ]
}
```

