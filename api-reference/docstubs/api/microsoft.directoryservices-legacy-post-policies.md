---
title: "Create policies"
description: "Create a new policies object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create policies

Namespace: Microsoft.DirectoryServices

Create a new policies object.

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
POST /legacy/policies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [policy](../resources/microsoft.directoryservices-policy.md) object.

The following table shows the properties that are required when you create the [policy](../resources/microsoft.directoryservices-policy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|alternativeIdentifier|String|**TODO: Add Description**|
|definition|String collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|isOrganizationDefault|Boolean|**TODO: Add Description**|
|keyCredentials|[keyCredential](../resources/microsoft.directoryservices-keycredential.md) collection|**TODO: Add Description**|
|type|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [policy](../resources/microsoft.directoryservices-policy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_policy_from_"
}
-->
``` http
POST https://graph.microsoft.com/changelog/legacy/policies
Content-Type: application/json
Content-length: 756

{
  "@odata.type": "#Microsoft.DirectoryServices.policy",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "alternativeIdentifier": "Alternative Identifier value",
  "definition": [
    "Definition value"
  ],
  "displayName": "Display Name value",
  "isOrganizationDefault": true,
  "keyCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.keyCredential",
      "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
      "endDateTime": "2017-01-01T00:01:58.2456509+00:00",
      "keyId": "c4860b27-0b27-c486-270b-86c4270b86c4",
      "startDateTime": "2017-01-01T00:01:26.5340071+00:00",
      "type": "Type value",
      "usage": "Usage value",
      "key": "a2V5"
    }
  ],
  "type": "Type value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.policy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.policy",
  "id": "5e2a1e9c-1e9c-5e2a-9c1e-2a5e9c1e2a5e",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "alternativeIdentifier": "Alternative Identifier value",
  "definition": [
    "Definition value"
  ],
  "displayName": "Display Name value",
  "isOrganizationDefault": true,
  "keyCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.keyCredential",
      "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
      "endDateTime": "2017-01-01T00:01:58.2456509+00:00",
      "keyId": "c4860b27-0b27-c486-270b-86c4270b86c4",
      "startDateTime": "2017-01-01T00:01:26.5340071+00:00",
      "type": "Type value",
      "usage": "Usage value",
      "key": "a2V5"
    }
  ],
  "type": "Type value"
}
```

