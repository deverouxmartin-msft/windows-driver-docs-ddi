---
UID: NS:d3dkmthk._D3DKMT_PRESENT_MULTIPLANE_OVERLAY3
title: _D3DKMT_PRESENT_MULTIPLANE_OVERLAY3
author: windows-driver-content
description: Contains present multiplane overlay information.
ms.assetid: 06f77522-57bd-41f7-b039-cd3dc10376d8
ms.author: windowsdriverdev
ms.date: 
ms.topic: struct
ms.prod: windows-hardware
ms.technology: windows-devices
ms.keywords: _D3DKMT_PRESENT_MULTIPLANE_OVERLAY3, D3DKMT_PRESENT_MULTIPLANE_OVERLAY3, 
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
req.typenames: D3DKMT_PRESENT_MULTIPLANE_OVERLAY3
topic_type: 
-	apiref
api_type: 
-	HeaderDef
api_location: 
-	d3dkmthk.h
api_name: 
-	_D3DKMT_PRESENT_MULTIPLANE_OVERLAY3
product:
-	Windows
targetos: Windows
---

# _D3DKMT_PRESENT_MULTIPLANE_OVERLAY3 structure

## -description

Contains present multiplane overlay information.

## -struct-fields

### -field hAdapter

A handle to the graphics adapter.

### -field ContextCount

The context count.

### -field pContextList

Pointer to a context list.

### -field VidPnSourceId

The zero-based identification number of the video present source in a path of a video present network (VidPN) topology that the monitor is connected to.

### -field PresentCount

The number of present operations that can be queued for the device that is specified by *hDevice*.

### -field Flags
 
### -field PresentPlaneCount

The number of resources to pin.

### -field ppPresentPlanes

Pointer to an array of present planes.

### -field pPostComposition

Pointer to post composition.

### -field Duration

Per-present duration. 

### -field HDRMetaDataType

The HDR metadata type.

### -field HDRMetaDataSize

The HDR metadata size.

### -field pHDRMetaData
 
The HDR metadata.

## -remarks

## -see-also