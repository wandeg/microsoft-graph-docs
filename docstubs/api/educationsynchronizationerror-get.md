---
title: "Get educationSynchronizationError"
description: "Read properties and relationships of the educationSynchronizationError object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get educationSynchronizationError

Namespace: microsoft.graph

Read properties and relationships of the [educationSynchronizationError](../resources/educationsynchronizationerror.md) object.

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
GET /education/synchronizationProfiles/{educationSynchronizationProfileId}/errors/{educationSynchronizationErrorId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [educationSynchronizationError](../resources/educationsynchronizationerror.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationsynchronizationerror"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{educationSynchronizationProfileId}/errors/{educationSynchronizationErrorId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 429

{
  "value": {
    "@odata.type": "#microsoft.graph.educationSynchronizationError",
    "id": "0ffc563d-563d-0ffc-3d56-fc0f3d56fc0f",
    "entryType": "Entry Type value",
    "errorCode": "Error Code value",
    "errorMessage": "Error Message value",
    "joiningValue": "Joining Value value",
    "recordedDateTime": "2016-12-31T23:58:55.0513559+00:00",
    "reportableIdentifier": "Reportable Identifier value"
  }
}
```

