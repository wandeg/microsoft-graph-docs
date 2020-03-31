---
title: "Add errors"
description: "Add errors by posting to the errors collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add errors

Namespace: microsoft.graph

Add errors by posting to the errors collection.

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
POST /education/synchronizationProfiles/{educationSynchronizationProfileId}/errors/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [educationSynchronizationError](../resources/educationsynchronizationerror.md) object.

The following table shows the properties that are required when you create the [educationSynchronizationError](../resources/educationsynchronizationerror.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|entryType|String||
|errorCode|String||
|errorMessage|String||
|joiningValue|String||
|recordedDateTime|DateTimeOffset||
|reportableIdentifier|String||



## Response
If successful, this method returns a `201 Created` response code and a [educationSynchronizationError](../resources/educationsynchronizationerror.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationsynchronizationerror_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{educationSynchronizationProfileId}/errors
Content-type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.educationSynchronizationError",
  "entryType": "Entry Type value",
  "errorCode": "Error Code value",
  "errorMessage": "Error Message value",
  "joiningValue": "Joining Value value",
  "recordedDateTime": "2016-12-31T23:58:59.1130037+03:00",
  "reportableIdentifier": "Reportable Identifier value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationsynchronizationerror"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.educationSynchronizationError",
  "id": "45f07c3b-7c3b-45f0-3b7c-f0453b7cf045",
  "entryType": "Entry Type value",
  "errorCode": "Error Code value",
  "errorMessage": "Error Message value",
  "joiningValue": "Joining Value value",
  "recordedDateTime": "2016-12-31T23:58:59.1130037+03:00",
  "reportableIdentifier": "Reportable Identifier value"
}
```

