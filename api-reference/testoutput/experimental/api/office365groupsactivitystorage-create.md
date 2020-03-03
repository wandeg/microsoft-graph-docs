---
title: "Create office365GroupsActivityStorage"
description: "Create a new office365GroupsActivityStorage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create office365GroupsActivityStorage

Namespace: microsoft.graph

Create a new [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) object.

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
POST ** Collection URI for microsoft.graph.office365GroupsActivityStorage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) object.

The following table shows the properties that are required when you create the [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|mailboxStorageUsedInBytes|Int64||
|siteStorageUsedInBytes|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_office365groupsactivitystorage_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.office365GroupsActivityStorage not found
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.office365GroupsActivityStorage",
  "reportRefreshDate": "Date",
  "mailboxStorageUsedInBytes": 9,
  "siteStorageUsedInBytes": 6,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365groupsactivitystorage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.office365GroupsActivityStorage",
  "id": "b54d6ca3-6ca3-b54d-a36c-4db5a36c4db5",
  "reportRefreshDate": "Date",
  "mailboxStorageUsedInBytes": 9,
  "siteStorageUsedInBytes": 6,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

