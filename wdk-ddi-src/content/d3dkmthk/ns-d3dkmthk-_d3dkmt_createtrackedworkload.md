---
UID: NS:d3dkmthk._D3DKMT_CREATETRACKEDWORKLOAD
title: _D3DKMT_CREATETRACKEDWORKLOAD
author: windows-driver-content
description: Arguments used to create a tracked workload.
ms.assetid: 53b93ab8-dbbe-4ef7-a7af-a4cae8d5221b
ms.author: windowsdriverdev
ms.date: 
ms.topic: struct
ms.prod: windows-hardware
ms.technology: windows-devices
ms.keywords: _D3DKMT_CREATETRACKEDWORKLOAD, D3DKMT_CREATETRACKEDWORKLOAD, 
req.header: d3dkmthk.h
req.include-header:
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib:
req.dll:
req.ddi-compliance:
req.unicode-ansi:
req.max-support:
req.typenames: D3DKMT_CREATETRACKEDWORKLOAD
topic_type: 
-	apiref
api_type: 
-	HeaderDef
api_location: 
-	d3dkmthk.h
api_name: 
-	_D3DKMT_CREATETRACKEDWORKLOAD
product:
-	Windows
targetos: Windows
tech.root: display
---

# _D3DKMT_CREATETRACKEDWORKLOAD structure

## -description

Arguments used to create a tracked workload.

## -struct-fields

### -field ContextCount

The number of contexts in *ContextArray*.

### -field ContextArray

Specifies context handles in which to create the workload.

### -field Flags

The flags to create this workload with.

### -field Policy

The policy to create this workload with.

### -field MaxInstances

Number of maximum simultaneous instances for this workload type.

### -field hResourceQueryTimestamps

Buffer which will contain the resolved query timestamps for the tracked workloads.

### -field hTrackedWorkload
 
The output handle for the workload.

## -remarks

## -see-also