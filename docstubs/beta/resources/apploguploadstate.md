---
title: "appLogUploadState enum type"
description: "AppLogUploadStatus"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# appLogUploadState enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

AppLogUploadStatus

## Members

| Member    | Value | Description                                                         |
| :-------- | ----: | :------------------------------------------------------------------ |
| pending   | 0     | Request is waiting to be processed or under processing              |
| completed | 1     | Request is completed with file uploaded to Azure blob for download. |
| failed    | 2     | Request finished processing and in error state.                     |