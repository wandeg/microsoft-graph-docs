---
title: "List errors"
description: "Get the educationSynchronizationErrors from the errors navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List errors

Namespace: microsoft.graph

Get the educationSynchronizationErrors from the errors navigation property.

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
GET /education/synchronizationProfiles/{educationSynchronizationProfileId}/errors
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationError](../resources/educationsynchronizationerror.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationsynchronizationerror"
}
-->
``` http
GET https://graph.microsoft.com/localtest/education/synchronizationProfiles/{educationSynchronizationProfileId}/errors
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationsynchronizationerror)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 459

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSynchronizationError",
      "id": "00e492eb-92eb-00e4-eb92-e400eb92e400",
      "entryType": "Entry Type value",
      "errorCode": "Error Code value",
      "errorMessage": "Error Message value",
      "joiningValue": "Joining Value value",
      "recordedDateTime": "2016-12-31T23:56:27.4887157+03:00",
      "reportableIdentifier": "Reportable Identifier value"
    }
  ]
}
```

