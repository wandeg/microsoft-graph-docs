---
title: "Add accessPackageResourceRequests"
description: "Add accessPackageResourceRequests by posting to the accessPackageResourceRequests collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add accessPackageResourceRequests

Namespace: microsoft.graph

Add accessPackageResourceRequests by posting to the accessPackageResourceRequests collection.

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
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.

The following table shows the properties that are required when you create the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|catalogId|String||
|executeImmediately|Boolean||
|isValidationOnly|Boolean||
|requestType|String||
|requestState|String||
|requestStatus|String||
|expirationDateTime|DateTimeOffset||
|justification|String||



## Response
If successful, this method returns a `201 Created` response code and a [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json
Content-length: 397

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRequest",
  "catalogId": "Catalog Id value",
  "executeImmediately": true,
  "isValidationOnly": true,
  "requestType": "Request Type value",
  "requestState": "Request State value",
  "requestStatus": "Request Status value",
  "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
  "justification": "Justification value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageresourcerequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 446

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRequest",
  "id": "5f7f21aa-21aa-5f7f-aa21-7f5faa217f5f",
  "catalogId": "Catalog Id value",
  "executeImmediately": true,
  "isValidationOnly": true,
  "requestType": "Request Type value",
  "requestState": "Request State value",
  "requestStatus": "Request Status value",
  "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
  "justification": "Justification value"
}
```

