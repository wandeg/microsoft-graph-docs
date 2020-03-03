---
title: "Update groupPolicyPresentationCheckBox"
description: "Update the properties of a groupPolicyPresentationCheckBox object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update groupPolicyPresentationCheckBox

Namespace: microsoft.graph

Update the properties of a [groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md) object.

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
PATCH ** Entity URI for microsoft.graph.groupPolicyPresentationCheckBox not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md) object.

The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|
|defaultChecked|Boolean|Default value for the check box. The default value is false.|



## Response
If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_grouppolicypresentationcheckbox"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.groupPolicyPresentationCheckBox not found
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
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
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "id": "7f1ce9d0-e9d0-7f1c-d0e9-1c7fd0e91c7f",
  "label": "Label value",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "defaultChecked": true
}
```

