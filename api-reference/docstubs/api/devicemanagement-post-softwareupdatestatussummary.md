---
title: "Add softwareUpdateStatusSummary"
description: "Add softwareUpdateStatusSummary by posting to the softwareUpdateStatusSummary collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Add softwareUpdateStatusSummary

Namespace: microsoft.graph

Add softwareUpdateStatusSummary by posting to the softwareUpdateStatusSummary collection.

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
POST /deviceManagement/softwareUpdateStatusSummary/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object.

The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|The name of the policy.|
|compliantDeviceCount|Int32|Number of compliant devices.|
|nonCompliantDeviceCount|Int32|Number of non compliant devices.|
|remediatedDeviceCount|Int32|Number of remediated devices.|
|errorDeviceCount|Int32|Number of devices had error.|
|unknownDeviceCount|Int32|Number of unknown devices.|
|conflictDeviceCount|Int32|Number of conflict devices.|
|notApplicableDeviceCount|Int32|Number of not applicable devices.|
|compliantUserCount|Int32|Number of compliant users.|
|nonCompliantUserCount|Int32|Number of non compliant users.|
|remediatedUserCount|Int32|Number of remediated users.|
|errorUserCount|Int32|Number of users had error.|
|unknownUserCount|Int32|Number of unknown users.|
|conflictUserCount|Int32|Number of conflict users.|
|notApplicableUserCount|Int32|Number of not applicable users.|



## Response
If successful, this method returns a `204 No Content` response code and a [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_softwareupdatestatussummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary/$ref
Content-Type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.softwareupdatestatussummary"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "9be5690f-690f-9be5-0f69-e59b0f69e59b",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

