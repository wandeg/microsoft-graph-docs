---
title: "Update applicationSignInDetailedSummary"
description: "Update the properties of an applicationSignInDetailedSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update applicationSignInDetailedSummary

Namespace: microsoft.graph

Update the properties of an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.

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
PATCH /reports/applicationSignInDetailedSummary/{applicationSignInDetailedSummaryId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.

The following table shows the properties that are required when you create the [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appId|String|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|status|[signInStatus](../resources/signinstatus.md)|**TODO: Add Description**|
|signInCount|Int64|**TODO: Add Description**|
|aggregatedEventDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_applicationsignindetailedsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/{applicationSignInDetailedSummaryId}
Content-Type: application/json
Content-length: 431

{
  "@odata.type": "#microsoft.graph.applicationSignInDetailedSummary",
  "appId": "App Id value",
  "appDisplayName": "App Display Name value",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus",
    "errorCode": 9,
    "failureReason": "Failure Reason value",
    "additionalDetails": "Additional Details value"
  },
  "signInCount": 11,
  "aggregatedEventDateTime": "2016-12-31T23:56:54.8139733+03:00"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.applicationSignInDetailedSummary",
  "id": "e60fdef5-def5-e60f-f5de-0fe6f5de0fe6",
  "appId": "App Id value",
  "appDisplayName": "App Display Name value",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus",
    "errorCode": 9,
    "failureReason": "Failure Reason value",
    "additionalDetails": "Additional Details value"
  },
  "signInCount": 11,
  "aggregatedEventDateTime": "2016-12-31T23:56:54.8139733+03:00"
}
```

