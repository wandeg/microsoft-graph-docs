---
title: "Add securityBaselineStates"
description: "Add securityBaselineStates by posting to the securityBaselineStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add securityBaselineStates

Namespace: microsoft.graph

Add securityBaselineStates by posting to the securityBaselineStates collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/managedDevices/{managedDeviceId}/securityBaselineStates/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [securityBaselineState](../resources/securitybaselinestate.md) object.

The following table shows the properties that are required when you create the [securityBaselineState](../resources/securitybaselinestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|securityBaselineTemplateId|String|The security baseline template id|
|displayName|String|The display name of the security baseline|



## Response
If successful, this method returns a `201 Created` response code and a [securityBaselineState](../resources/securitybaselinestate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_securitybaselinestate_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/managedDevices/{managedDeviceId}/securityBaselineStates
Content-type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securitybaselinestate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 224

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "2aaf15ab-15ab-2aaf-ab15-af2aab15af2a",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```

