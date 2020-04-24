---
title: "Update securityBaselineStates"
description: "Update the properties of a securityBaselineStates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update securityBaselineStates

Namespace: microsoft.graph

Update the properties of a securityBaselineStates object.

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
PATCH /invitations/{invitationsId}/invitedUser/managedDevices/{managedDeviceId}/securityBaselineStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [securityBaselineState](../resources/securitybaselinestate.md) object.

The following table shows the properties that are required when you create the [securityBaselineState](../resources/securitybaselinestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|securityBaselineTemplateId|String|The security baseline template id|
|displayName|String|The display name of the security baseline|



## Response
If successful, this method returns a `200 OK` response code and an updated [securityBaselineState](../resources/securitybaselinestate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_securitybaselinestates"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/managedDevices/{managedDeviceId}/securityBaselineStates
Content-Type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
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
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "c8377e3d-7e3d-c837-3d7e-37c83d7e37c8",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```

