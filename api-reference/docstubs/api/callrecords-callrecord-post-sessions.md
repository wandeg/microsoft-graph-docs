---
title: "Create sessions"
description: "Create a new sessions object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create sessions

Namespace: microsoft.graph.callRecords

Create a new sessions object.

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
POST /communications/callRecords/{callRecordId}/sessions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [session](../resources/callrecords-session.md) object.

The following table shows the properties that are required when you create the [session](../resources/callrecords-session.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/callrecords-entity.md)|
|modalities|modality collection|**TODO: Add Description**. Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|caller|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|callee|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|failureInfo|[failureInfo](../resources/callrecords-failureinfo.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [session](../resources/callrecords-session.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_session_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/communications/callRecords/{callRecordId}/sessions
Content-Type: application/json
Content-length: 707

{
  "@odata.type": "#microsoft.graph.callRecords.session",
  "modalities": [
    "String"
  ],
  "startDateTime": "2017-01-01T00:01:28.8507081+03:00",
  "endDateTime": "2017-01-01T00:02:50.4198958+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.callrecords.session"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.callRecords.session",
  "id": "d4748e05-8e05-d474-058e-74d4058e74d4",
  "modalities": [
    "String"
  ],
  "startDateTime": "2017-01-01T00:01:28.8507081+03:00",
  "endDateTime": "2017-01-01T00:02:50.4198958+03:00",
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

