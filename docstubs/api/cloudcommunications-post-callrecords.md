---
title: "Add callRecords"
description: "Add callRecords by posting to the callRecords collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add callRecords

Namespace: microsoft.graph.callRecords

Add callRecords by posting to the callRecords collection.

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
POST /communications/callRecords/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [callRecord](../resources/callrecords-callrecord.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_callrecord_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/communications/callRecords
Content-type: application/json
Content-length: 766

{
  "@odata.type": "#microsoft.graph.callRecords.callRecord",
  "version": 7,
  "type": "String",
  "modalities": [
    "String"
  ],
  "startDateTime": "2017-01-01T00:03:01.5077011+03:00",
  "endDateTime": "2016-12-31T23:58:47.6569305+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.callrecords.callrecord"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 878

{
  "@odata.type": "#microsoft.graph.callRecords.callRecord",
  "id": "ac288cd2-8cd2-ac28-d28c-28acd28c28ac",
  "version": 7,
  "type": "String",
  "modalities": [
    "String"
  ],
  "lastModifiedDateTime": "2017-01-01T00:01:28.872294+03:00",
  "startDateTime": "2017-01-01T00:03:01.5077011+03:00",
  "endDateTime": "2016-12-31T23:58:47.6569305+03:00",
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

