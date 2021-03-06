---
UID: NC:d3dkmthk.PFND3DKMT_SHAREDPRIMARYLOCKNOTIFICATION
title: PFND3DKMT_SHAREDPRIMARYLOCKNOTIFICATION
author: windows-driver-content
description: The PFND3DKMT_SHAREDPRIMARYLOCKNOTIFICATION callback function notifies the operating system about an upcoming lock to a shared primary surface.
ms.assetid: ceb858a0-a82b-4649-9a97-884cdf09b822
ms.author: windowsdriverdev
ms.date: 
ms.topic: callback
ms.prod: windows-hardware
ms.technology: windows-devices
req.header: d3dkmthk.h
req.include-header:
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib:
req.dll:
req.irql: 
req.ddi-compliance:
req.unicode-ansi:
req.idl:
req.max-support:
req.namespace:
req.assembly:
req.type-library: 
topic_type: 
-	apiref
api_type: 
-	UserDefined
api_location: 
-	d3dkmthk.h
api_name: 
-	PFND3DKMT_SHAREDPRIMARYLOCKNOTIFICATION
product:
-	Windows
targetos: Windows
---

# PFND3DKMT_SHAREDPRIMARYLOCKNOTIFICATION callback function

## -description

The PFND3DKMT_SHAREDPRIMARYLOCKNOTIFICATION callback function notifies the operating system about an upcoming lock to a shared primary surface.

## -prototype

```
//Declaration

PFND3DKMT_SHAREDPRIMARYLOCKNOTIFICATION Pfnd3dkmtSharedprimarylocknotification; 

// Definition

NTSTATUS Pfnd3dkmtSharedprimarylocknotification 
(
	const D3DKMT_SHAREDPRIMARYLOCKNOTIFICATION *
)
{...}

```

## -parameters

### -param * 

Pointer to a [D3DKMT_SHAREDPRIMARYLOCKNOTIFICATION](ns-d3dkmthk-_d3dkmt_sharedprimarylocknotification.md) structure.

## -returns

Returns NTSTATUS.


## -remarks




## -see-also