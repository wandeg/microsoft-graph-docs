---
title: "Add groupLifecyclePolicies"
description: "Add groupLifecyclePolicies by posting to the groupLifecyclePolicies collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add groupLifecyclePolicies

Namespace: microsoft.graph

Add groupLifecyclePolicies by posting to the groupLifecyclePolicies collection.

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
POST /groups/{groupsId}/groupLifecyclePolicies/$ref
POST /me/joinedGroups/{groupId}/groupLifecyclePolicies/$ref
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
  "id": "0e535f2a-5f2a-0e53-2a5f-530e2a5f530e",
  "groupLifetimeInDays": 3,
  "managedGroupTypes": "Managed Group Types value",
  "alternateNotificationEmails": "Alternate Notification Emails value"
}
```

