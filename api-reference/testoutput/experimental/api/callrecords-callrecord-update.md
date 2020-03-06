---
title: "Update callRecord"
description: "Update the properties of a callRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update callRecord

Namespace: microsoft.graph.callRecords

Update the properties of a [callRecord](../resources/callrecords-callrecord.md) object.

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
PATCH /communications/callRecords/{callRecordId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [callRecord](../resources/callrecords-callrecord.md) object.

The following table shows the properties that are required when you create the [callRecord](../resources/callrecords-callrecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/callrecords-entity.md)|
|version|Int64||
|type|Enumeration|. Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|modalities|Enumeration collection|. Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|lastModifiedDateTime|DateTimeOffset||
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|organizer|[identitySet](../resources/callrecords-identityset.md)||
|participants|[identitySet](../resources/callrecords-identityset.md) collection||
|joinWebUrl|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [callRecord](../resources/callrecords-callrecord.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_callrecord"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/communications/callRecords/{callRecordId}
Content-type: application/json
Content-length: 765

{
  "@odata.type": "#microsoft.graph.callRecords.callRecord",
  "version": 7,
  "type": "String",
  "modalities": [
    "String"
  ],
  "startDateTime": "2017-01-01T00:00:14.2767228+03:00",
  "endDateTime": "2017-01-01T00:02:18.392989+03:00",
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
Content-Length: 878

{
  "@odata.type": "#microsoft.graph.callRecords.callRecord",
  "id": "7262929a-929a-7262-9a92-62729a926272",
  "version": 7,
  "type": "String",
  "modalities": [
    "String"
  ],
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
  "startDateTime": "2017-01-01T00:00:14.2767228+03:00",
  "endDateTime": "2017-01-01T00:02:18.392989+03:00",
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
```

