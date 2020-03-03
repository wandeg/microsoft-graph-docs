---
title: "Add sessions"
description: "Add sessions by posting to the sessions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add sessions

Namespace: microsoft.graph.callRecords

Add sessions by posting to the sessions collection.

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
POST /communications/callRecords/{callRecordId}/sessions/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [session](../resources/callrecords-session.md) object.

The following table shows the properties that are required when you create the [session](../resources/callrecords-session.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/callrecords-entity.md)|
|modalities|Enumeration collection|. Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|caller|[endpoint](../resources/callrecords-endpoint.md)||
|callee|[endpoint](../resources/callrecords-endpoint.md)||
|failureInfo|[failureInfo](../resources/callrecords-failureinfo.md)||



## Response
If successful, this method returns a `201 Created` response code and a [session](../resources/callrecords-session.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_session_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/communications/callRecords/{callRecordId}/sessions
Content-type: application/json
Content-length: 707

{
  "@odata.type": "#microsoft.graph.callRecords.session",
  "modalities": [
    "String"
  ],
  "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
  "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
  "caller": {
    "@odata.type": "microsoft.graph.callRecords.endpoint",
    "userAgent": {
      "@odata.type": "microsoft.graph.callRecords.userAgent",
      "headerValue": "Header Value value",
      "applicationVersion": "Application Version value"
    }
  },
  "callee": {
    "@odata.type": "microsoft.graph.callRecords.endpoint"
  },
  "failureInfo": {
    "@odata.type": "microsoft.graph.callRecords.failureInfo",
    "stage": "String",
    "reason": "Reason value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callrecords.session"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 756

{
  "@odata.type": "#microsoft.graph.callRecords.session",
  "id": "26004e0a-4e0a-2600-0a4e-00260a4e0026",
  "modalities": [
    "String"
  ],
  "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
  "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
  "caller": {
    "@odata.type": "microsoft.graph.callRecords.endpoint",
    "userAgent": {
      "@odata.type": "microsoft.graph.callRecords.userAgent",
      "headerValue": "Header Value value",
      "applicationVersion": "Application Version value"
    }
  },
  "callee": {
    "@odata.type": "microsoft.graph.callRecords.endpoint"
  },
  "failureInfo": {
    "@odata.type": "microsoft.graph.callRecords.failureInfo",
    "stage": "String",
    "reason": "Reason value"
  }
}
```

