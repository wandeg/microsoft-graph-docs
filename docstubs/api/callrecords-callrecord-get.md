---
title: "Get callRecord"
description: "Read properties and relationships of a callRecord object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get callRecord

Namespace: microsoft.graph.callRecords

Read properties and relationships of a [callRecord](../resources/callrecords-callrecord.md) object.

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
GET /communications/callRecords/{callRecordId}
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
If successful, this method returns a `200 OK` response code and a [callRecord](../resources/callrecords-callrecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_callrecord"
}
-->
``` http
GET https://graph.microsoft.com/beta/communications/callRecords/{callRecordId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.callRecord"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.callRecords.callRecord",
    "id": "400185c3-85c3-4001-c385-0140c3850140",
    "version": 7,
    "type": "String",
    "modalities": [
      "String"
    ],
    "lastModifiedDateTime": "2017-01-01T00:01:44.3371159+03:00",
    "startDateTime": "2017-01-01T00:03:24.4987822+03:00",
    "endDateTime": "2016-12-31T23:59:38.6819041+03:00",
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
}
```

