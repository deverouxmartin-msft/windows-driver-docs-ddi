---
UID: NS:d3dkmthk._D3DKMT_GETAVAILABLETRACKEDWORKLOADINDEX
title: _D3DKMT_GETAVAILABLETRACKEDWORKLOADINDEX
author: windows-driver-content
description: Gets the available tracked workload index.
ms.assetid: 8a64867d-86b3-4d6e-a029-06ae7437133b
ms.author: windowsdriverdev
ms.date: 
ms.topic: struct
ms.prod: windows-hardware
ms.technology: windows-devices
ms.keywords: _D3DKMT_GETAVAILABLETRACKEDWORKLOADINDEX, D3DKMT_GETAVAILABLETRACKEDWORKLOADINDEX, 
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
req.typenames: D3DKMT_GETAVAILABLETRACKEDWORKLOADINDEX
topic_type: 
-	apiref
api_type: 
-	HeaderDef
api_location: 
-	d3dkmthk.h
api_name: 
-	_D3DKMT_GETAVAILABLETRACKEDWORKLOADINDEX
product:
-	Windows
targetos: Windows
tech.root: display
---

# _D3DKMT_GETAVAILABLETRACKEDWORKLOADINDEX structure

## -description

Gets the available tracked workload index.

## -struct-fields

### -field hDevice

A handle to the device context.

### -field hTrackedWorkload

A handle to the tracked workload instance.

### -field FenceCompletedValue

The fence value for the completed workloads.

### -field AvailableTrackedWorkloadIndex
 
[out] The first available tracked workload index.

## -remarks

## -see-also