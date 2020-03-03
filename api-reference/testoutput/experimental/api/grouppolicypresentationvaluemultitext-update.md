---
title: "Update groupPolicyPresentationValueMultiText"
description: "Update the properties of a groupPolicyPresentationValueMultiText object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update groupPolicyPresentationValueMultiText

Namespace: microsoft.graph

Update the properties of a [groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.graph.groupPolicyPresentationValueMultiText not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md) object.

The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the object was last modified. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|The date and time the object was created. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|
|values|String collection|A collection of non-empty strings for the associated presentation.|



## Response
If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_grouppolicypresentationvaluemultitext"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.groupPolicyPresentationValueMultiText not found
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "id": "0cdf0197-0197-0cdf-9701-df0c9701df0c",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "values": [
    "Values value"
  ]
}
```

