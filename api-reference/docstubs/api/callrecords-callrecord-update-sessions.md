---
title: "Update sessions"
description: "Update the properties of a sessions object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update sessions

Namespace: microsoft.graph.callRecords

Update the properties of a sessions object.

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
PATCH /communications/callRecords/{callRecordId}/sessions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [session](../resources/callrecords-session.md) object.

The following table shows the properties that are required when you create the [session](../resources/callrecords-session.md).

|Property|Type|Description|
|:---|:---|:---|
|modalities|modality collection|**TODO: Add Description**. Possible values are: `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|caller|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|callee|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|failureInfo|[failureInfo](../resources/callrecords-failureinfo.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [session](../resources/callrecords-session.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_sessions"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/communications/callRecords/{callRecordId}/sessions
Content-Type: application/json
Content-length: 707

{
  "@odata.type": "#microsoft.graph.callRecords.session",
  "modalities": [
    "String"
  ],
  "startDateTime": "2016-12-31T23:56:48.8437798+03:00",
  "endDateTime": "2016-12-31T23:57:13.0779697+03:00",
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.callRecords.session",
  "modalities": [
    "String"
  ],
  "startDateTime": "2016-12-31T23:56:48.8437798+03:00",
  "endDateTime": "2016-12-31T23:57:13.0779697+03:00",
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
  },
  "id": "f87014cc-14cc-f870-cc14-70f8cc1470f8"
}
```

