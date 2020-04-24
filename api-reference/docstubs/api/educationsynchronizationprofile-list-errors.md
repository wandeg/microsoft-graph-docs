---
title: "List errors"
description: "Get the educationSynchronizationErrors from the errors navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List errors

Namespace: microsoft.graph

Get the educationSynchronizationErrors from the errors navigation property.

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
GET /education/synchronizationProfiles/{educationSynchronizationProfileId}/errors
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationError](../resources/educationsynchronizationerror.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationsynchronizationerror"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{educationSynchronizationProfileId}/errors
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationsynchronizationerror)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

