---
title: "Update deviceConfigurationUserStateSummary"
description: "Update the properties of a deviceConfigurationUserStateSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceConfigurationUserStateSummary

Namespace: microsoft.graph

Update the properties of a [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) object.

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
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) object.

The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|unknownUserCount|Int32|Number of unknown users|
|notApplicableUserCount|Int32|Number of not applicable users|
|compliantUserCount|Int32|Number of compliant users|
|remediatedUserCount|Int32|Number of remediated users|
|nonCompliantUserCount|Int32|Number of NonCompliant users|
|errorUserCount|Int32|Number of error users|
|conflictUserCount|Int32|Number of conflict users|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_deviceconfigurationuserstatesummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-Type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
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
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "797ebcaf-bcaf-797e-afbc-7e79afbc7e79",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```

