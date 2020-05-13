---
title: "Update telecomExpenseManagementPartners"
description: "Update the properties of a telecomExpenseManagementPartners object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update telecomExpenseManagementPartners

Namespace: microsoft.graph

Update the properties of a telecomExpenseManagementPartners object.

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
PATCH /deviceManagement/telecomExpenseManagementPartners
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [telecomExpenseManagementPartner](../resources/intune-telecomexpensemanagementpartner.md) object.

The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-telecomexpensemanagementpartner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|url|String|**TODO: Add Description**|
|appAuthorized|Boolean|**TODO: Add Description**|
|enabled|Boolean|**TODO: Add Description**|
|lastConnectionDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-telecomexpensemanagementpartner.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_telecomexpensemanagementpartners"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
Content-Type: application/json
Content-length: 228

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "String",
  "url": "String",
  "appAuthorized": "Boolean",
  "enabled": "Boolean",
  "lastConnectionDateTime": "String (timestamp)"
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
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "ab6bcbe5-cbe5-ab6b-e5cb-6babe5cb6bab",
  "displayName": "String",
  "url": "String",
  "appAuthorized": "Boolean",
  "enabled": "Boolean",
  "lastConnectionDateTime": "String (timestamp)"
}
```

