---
title: "Update appConsentRequest"
description: "Update the properties of a appConsentRequest object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update appConsentRequest

Namespace: microsoft.graph

Update the properties of a [appConsentRequest](../resources/appconsentrequest.md) object.

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
PATCH /me/appConsentRequestsForApproval/{appConsentRequestId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [appConsentRequest](../resources/appconsentrequest.md) object.

The following table shows the properties that are required when you create the [appConsentRequest](../resources/appconsentrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appId|String|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|consentType|String|**TODO: Add Description**|
|pendingScopes|[appConsentRequestScope](../resources/appconsentrequestscope.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [appConsentRequest](../resources/appconsentrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_appconsentrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/appConsentRequestsForApproval/{appConsentRequestId}
Content-Type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.appConsentRequest",
  "appId": "App Id value",
  "appDisplayName": "App Display Name value",
  "consentType": "Consent Type value",
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope",
      "displayName": "Display Name value"
    }
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.appConsentRequest",
  "id": "66359143-9143-6635-4391-356643913566",
  "appId": "App Id value",
  "appDisplayName": "App Display Name value",
  "consentType": "Consent Type value",
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope",
      "displayName": "Display Name value"
    }
  ]
}
```

