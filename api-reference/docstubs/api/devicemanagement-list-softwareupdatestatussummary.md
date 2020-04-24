---
title: "List softwareUpdateStatusSummary"
description: "Get the softwareUpdateStatusSummaries from the softwareUpdateStatusSummary navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List softwareUpdateStatusSummary

Namespace: microsoft.graph

Get the softwareUpdateStatusSummaries from the softwareUpdateStatusSummary navigation property.

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
GET /deviceManagement/softwareUpdateStatusSummary
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
If successful, this method returns a `200 OK` response code and a collection of [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_softwareupdatestatussummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.softwareupdatestatussummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
      "id": "96bfc878-c878-96bf-78c8-bf9678c8bf96",
      "displayName": "Display Name value",
      "compliantDeviceCount": 4,
      "nonCompliantDeviceCount": 7,
      "remediatedDeviceCount": 5,
      "errorDeviceCount": 0,
      "unknownDeviceCount": 2,
      "conflictDeviceCount": 3,
      "notApplicableDeviceCount": 8,
      "compliantUserCount": 2,
      "nonCompliantUserCount": 5,
      "remediatedUserCount": 3,
      "errorUserCount": 14,
      "unknownUserCount": 0,
      "conflictUserCount": 1,
      "notApplicableUserCount": 6
    }
  ]
}
```

