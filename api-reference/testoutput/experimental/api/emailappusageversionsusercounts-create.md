---
title: "Create emailAppUsageVersionsUserCounts"
description: "Create a new emailAppUsageVersionsUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create emailAppUsageVersionsUserCounts

Namespace: microsoft.graph

Create a new [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.emailAppUsageVersionsUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) object.

The following table shows the properties that are required when you create the [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|outlook2016|Int64||
|outlook2013|Int64||
|outlook2010|Int64||
|outlook2007|Int64||
|undetermined|Int64||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_emailappusageversionsusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.emailAppUsageVersionsUserCounts not found
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.emailAppUsageVersionsUserCounts",
  "reportRefreshDate": "Date",
  "outlook2016": 11,
  "outlook2013": 11,
  "outlook2010": 11,
  "outlook2007": 11,
  "undetermined": 12,
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailappusageversionsusercounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.emailAppUsageVersionsUserCounts",
  "id": "908104c9-04c9-9081-c904-8190c9048190",
  "reportRefreshDate": "Date",
  "outlook2016": 11,
  "outlook2013": 11,
  "outlook2010": 11,
  "outlook2007": 11,
  "undetermined": 12,
  "reportPeriod": "Report Period value"
}
```

