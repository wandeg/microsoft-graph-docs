---
title: "Create deviceConfigurationUserStateSummaries"
description: "Create a new deviceConfigurationUserStateSummaries object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceConfigurationUserStateSummaries

Namespace: microsoft.graph

Create a new deviceConfigurationUserStateSummaries object.

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
POST /deviceManagement/deviceConfigurationUserStateSummaries
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) object.

The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|unknownUserCount|Int32|**TODO: Add Description**|
|notApplicableUserCount|Int32|**TODO: Add Description**|
|compliantUserCount|Int32|**TODO: Add Description**|
|remediatedUserCount|Int32|**TODO: Add Description**|
|nonCompliantUserCount|Int32|**TODO: Add Description**|
|errorUserCount|Int32|**TODO: Add Description**|
|conflictUserCount|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStateSummary](../resources/deviceconfigurationuserstatesummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_deviceconfigurationuserstatesummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-Type: application/json
Content-length: 330

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "unknownUserCount": "Integer",
  "notApplicableUserCount": "Integer",
  "compliantUserCount": "Integer",
  "remediatedUserCount": "Integer",
  "nonCompliantUserCount": "Integer",
  "errorUserCount": "Integer",
  "conflictUserCount": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceconfigurationuserstatesummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "63e6959d-959d-63e6-9d95-e6639d95e663",
  "unknownUserCount": "Integer",
  "notApplicableUserCount": "Integer",
  "compliantUserCount": "Integer",
  "remediatedUserCount": "Integer",
  "nonCompliantUserCount": "Integer",
  "errorUserCount": "Integer",
  "conflictUserCount": "Integer"
}
```

