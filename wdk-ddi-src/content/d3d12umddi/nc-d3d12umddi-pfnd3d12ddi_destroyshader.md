---
UID: NC:d3d12umddi.PFND3D12DDI_DESTROYSHADER
title: PFND3D12DDI_DESTROYSHADER
author: windows-driver-content
description: Destroy shader.
ms.assetid: 11ca0734-50b5-45a3-af8a-d344c88a2b68
ms.author: windowsdriverdev
ms.date: 
ms.topic: callback
ms.prod: windows-hardware
ms.technology: windows-devices
req.header: d3d12umddi.h
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
-	d3d12umddi.h
api_name: 
-	PFND3D12DDI_DESTROYSHADER
product: 
- Windows
targetos: Windows
tech.root: display
---

# PFND3D12DDI_DESTROYSHADER callback function

## -description

Destroy shader.

## -prototype

```
//Declaration

PFND3D12DDI_DESTROYSHADER Pfnd3d12ddiDestroyshader; 

// Definition

VOID Pfnd3d12ddiDestroyshader 
(
	 D3D12DDI_HDEVICE
	 D3D12DDI_HSHADER
)
{...}

PFND3D12DDI_DESTROYSHADER 


```

## -parameters

### -param D3D12DDI_HDEVICE  

A handle to the display device (graphics context).
 
### -param D3D12DDI_HSHADER: 

A shader handle.

## -returns

Returns VOID.

## -remarks




## -see-also