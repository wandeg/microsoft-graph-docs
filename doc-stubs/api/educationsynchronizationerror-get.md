---
title: "Get educationSynchronizationError"
description: "Read the properties and relationships of an educationSynchronizationError object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get educationSynchronizationError

Namespace: microsoft.graph

Read the properties and relationships of an [educationSynchronizationError](../resources/educationsynchronizationerror.md) object.

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
GET /education/synchronizationProfiles/{educationSynchronizationProfileId}/errors/{educationSynchronizationErrorId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [educationSynchronizationError](../resources/educationsynchronizationerror.md) object in the response body.

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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.educationSynchronizationError",
    "id": "4a6ac45e-c45e-4a6a-5ec4-6a4a5ec46a4a",
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "String (timestamp)",
    "reportableIdentifier": "String"
  }
}
```

