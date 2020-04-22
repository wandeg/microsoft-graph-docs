---
title: "Create groupLifecyclePolicies"
description: "Create a new groupLifecyclePolicies object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create groupLifecyclePolicies

Namespace: microsoft.graph

Create a new groupLifecyclePolicies object.

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
POST /groups/{groupsId}/groupLifecyclePolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.

The following table shows the properties that are required when you create the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|groupLifetimeInDays|Int32|**TODO: Add Description**|
|managedGroupTypes|String|**TODO: Add Description**|
|alternateNotificationEmails|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_grouplifecyclepolicies"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/groupLifecyclePolicies
Content-Type: application/json
Content-length: 217

{
  "@odata.type": "#microsoft.graph.groupLifecyclePolicy",
  "groupLifetimeInDays": 3,
  "managedGroupTypes": "Managed Group Types value",
  "alternateNotificationEmails": "Alternate Notification Emails value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.grouplifecyclepolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.groupLifecyclePolicy",
  "id": "76f53f5a-3f5a-76f5-5a3f-f5765a3ff576",
  "groupLifetimeInDays": 3,
  "managedGroupTypes": "Managed Group Types value",
  "alternateNotificationEmails": "Alternate Notification Emails value"
}
```

