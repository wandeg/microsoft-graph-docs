---
title: "Create errors"
description: "Create a new errors object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create errors

Namespace: microsoft.graph

Create a new errors object.

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
POST /education/synchronizationProfiles/{educationSynchronizationProfileId}/errors
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [educationSynchronizationError](../resources/educationsynchronizationerror.md) object.

The following table shows the properties that are required when you create the [educationSynchronizationError](../resources/educationsynchronizationerror.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|entryType|String|**TODO: Add Description**|
|errorCode|String|**TODO: Add Description**|
|errorMessage|String|**TODO: Add Description**|
|joiningValue|String|**TODO: Add Description**|
|recordedDateTime|DateTimeOffset|**TODO: Add Description**|
|reportableIdentifier|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [educationSynchronizationError](../resources/educationsynchronizationerror.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationsynchronizationerror_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{educationSynchronizationProfileId}/errors
Content-Type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.educationSynchronizationError",
  "entryType": "Entry Type value",
  "errorCode": "Error Code value",
  "errorMessage": "Error Message value",
  "joiningValue": "Joining Value value",
  "recordedDateTime": "2016-12-31T23:56:35.2919298+03:00",
  "reportableIdentifier": "Reportable Identifier value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationsynchronizationerror"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationError",
  "id": "076ddbe8-dbe8-076d-e8db-6d07e8db6d07",
  "entryType": "Entry Type value",
  "errorCode": "Error Code value",
  "errorMessage": "Error Message value",
  "joiningValue": "Joining Value value",
  "recordedDateTime": "2016-12-31T23:56:35.2919298+03:00",
  "reportableIdentifier": "Reportable Identifier value"
}
```

