---
title: "Update privilegedRoleSummary"
description: "Update the properties of a privilegedRoleSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update privilegedRoleSummary

Namespace: microsoft.graph

Update the properties of a [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.

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
PATCH /privilegedRoles/{privilegedRolesId}/summary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.

The following table shows the properties that are required when you create the [privilegedRoleSummary](../resources/privilegedrolesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|roleSummaryStatus|**TODO: Add Description**. Possible values are: `ok`, `bad`.|
|usersCount|Int32|**TODO: Add Description**|
|managedCount|Int32|**TODO: Add Description**|
|elevatedCount|Int32|**TODO: Add Description**|
|mfaEnabled|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_privilegedrolesummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedRoles/{privilegedRolesId}/summary
Content-Type: application/json
Content-length: 177

{
  "@odata.type": "#microsoft.graph.privilegedRoleSummary",
  "status": "String",
  "usersCount": 10,
  "managedCount": 12,
  "elevatedCount": 13,
  "mfaEnabled": true
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
  "@odata.type": "#microsoft.graph.privilegedRoleSummary",
  "id": "ae377179-7179-ae37-7971-37ae797137ae",
  "status": "String",
  "usersCount": 10,
  "managedCount": 12,
  "elevatedCount": 13,
  "mfaEnabled": true
}
```

