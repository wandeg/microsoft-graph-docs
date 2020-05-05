---
title: "Create policies"
description: "Create a new policies object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create policies

Namespace: microsoft.cpim.api.dataModels

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
POST /trustFramework/policies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [trustFrameworkPolicy](../resources/microsoft.cpim.api.datamodels-trustframeworkpolicy.md) object.

The following table shows the properties that are required when you create the [trustFrameworkPolicy](../resources/microsoft.cpim.api.datamodels-trustframeworkpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [trustFrameworkPolicy](../resources/microsoft.cpim.api.datamodels-trustframeworkpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/trustFramework/policies
Content-Type: application/json
Content-length: 76

{
  "@odata.type": "#microsoft.cpim.api.dataModels.trustFrameworkPolicy"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.cpim.api.datamodels.trustframeworkpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.cpim.api.dataModels.trustFrameworkPolicy",
  "id": "79ab9528-9528-79ab-2895-ab792895ab79"
}
```

