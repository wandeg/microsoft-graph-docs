---
title: "deviceHealthScriptRunSummary resource type"
description: "Contains properties for the run summary of a device management script."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceHealthScriptRunSummary resource type


Namespace: microsoft.graph

Contains properties for the run summary of a device management script.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceHealthScriptRunSummaries](../api/intune-devices-devicehealthscriptrunsummary-list.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) collection|List properties and relationships of the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) objects.|
|[Get deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.|
|[Create deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-create.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Create a new [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.|
|[Delete deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-delete.md)|None|Deletes a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).|
|[Update deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|detectionScriptErrorDeviceCount|Int32|Number of devices on which the detection script execution encountered an error and did not complete|
|detectionScriptPendingDeviceCount|Int32|Number of devices which have not yet run the latest version of the device health script|
|id|String| Inherited from [entity](../resources/entity.md)|
|issueDetectedDeviceCount|Int32|Number of devices for which the detection script found an issue|
|issueRemediatedCumulativeDeviceCount|Int32|Number of devices that were remediated over the last 30 days|
|issueRemediatedDeviceCount|Int32|Number of devices for which the remediation script was able to resolve the detected issue|
|issueReoccurredDeviceCount|Int32|Number of devices for which the remediation script executed successfully but failed to resolve the detected issue|
|lastScriptRunDateTime|DateTimeOffset|Last run time for the script across all devices|
|noIssueDetectedDeviceCount|Int32|Number of devices for which the detection script did not find an issue and the device is healthy|
|remediationScriptErrorDeviceCount|Int32|Number of devices for which the remediation script execution encountered an error and did not complete|
|remediationSkippedDeviceCount|Int32|Number of devices for which remediation was skipped|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```

