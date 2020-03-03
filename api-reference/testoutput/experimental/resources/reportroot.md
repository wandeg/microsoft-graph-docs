---
title: "reportRoot resource type"
description: "The resource that represents an instance of History Reports."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# reportRoot resource type


Namespace: microsoft.graph

The resource that represents an instance of History Reports.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List reportRoots](../api/reportroot-list.md)|[reportRoot](../resources/reportroot.md) collection|List properties and relationships of the [reportRoot](../resources/reportroot.md) objects.|
|[Get reportRoot](../api/reportroot-get.md)|[reportRoot](../resources/reportroot.md)|Read properties and relationships of the [reportRoot](../resources/reportroot.md) object.|
|[Create reportRoot](../api/reportroot-create.md)|[reportRoot](../resources/reportroot.md)|Create a new [reportRoot](../resources/reportroot.md) object.|
|[Delete reportRoot](../api/reportroot-delete.md)|None|Deletes a [reportRoot](../resources/reportroot.md).|
|[Update reportRoot](../api/reportroot-update.md)|[reportRoot](../resources/reportroot.md)|Update the properties of a [reportRoot](../resources/reportroot.md) object.|
|[deviceConfigurationUserActivity](../api/reportroot-deviceconfigurationuseractivity.md)|[report](../resources/report.md)||
|[deviceConfigurationDeviceActivity](../api/reportroot-deviceconfigurationdeviceactivity.md)|[report](../resources/report.md)||
|[managedDeviceEnrollmentFailureDetails](../api/reportroot-manageddeviceenrollmentfailuredetails.md)|[report](../resources/report.md)||
|[managedDeviceEnrollmentFailureDetails](../api/reportroot-manageddeviceenrollmentfailuredetails.md)|[report](../resources/report.md)||
|[managedDeviceEnrollmentFailureTrends](../api/reportroot-manageddeviceenrollmentfailuretrends.md)|[report](../resources/report.md)||
|[managedDeviceEnrollmentTopFailures](../api/reportroot-manageddeviceenrollmenttopfailures.md)|[report](../resources/report.md)||
|[managedDeviceEnrollmentTopFailures](../api/reportroot-manageddeviceenrollmenttopfailures.md)|[report](../resources/report.md)||
|[managedDeviceEnrollmentAbandonmentSummary](../api/reportroot-manageddeviceenrollmentabandonmentsummary.md)|[report](../resources/report.md)||
|[managedDeviceEnrollmentAbandonmentDetails](../api/reportroot-manageddeviceenrollmentabandonmentdetails.md)|[report](../resources/report.md)||
|[List applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) collection|Get the applicationSignInDetailedSummaries from the applicationSignInDetailedSummary navigation property.|
|[Add applicationSignInDetailedSummary](../api/reportroot-post-applicationsignindetailedsummary.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Add applicationSignInDetailedSummary by posting to the applicationSignInDetailedSummary collection.|
|[List credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md)|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) collection|Get the credentialUserRegistrationDetailses from the credentialUserRegistrationDetails navigation property.|
|[Add credentialUserRegistrationDetails](../api/reportroot-post-credentialuserregistrationdetails.md)|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Add credentialUserRegistrationDetails by posting to the credentialUserRegistrationDetails collection.|
|[List userCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md) collection|Get the userCredentialUsageDetailses from the userCredentialUsageDetails navigation property.|
|[Add userCredentialUsageDetails](../api/reportroot-post-usercredentialusagedetails.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Add userCredentialUsageDetails by posting to the userCredentialUsageDetails collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|applicationSignInDetailedSummary|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) collection||
|credentialUserRegistrationDetails|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) collection||
|userCredentialUsageDetails|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

