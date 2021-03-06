---
UID: NC:vmbuskernelmodeclientlibapi.FN_VMB_CHANNEL_PACKET_FAIL
title: FN_VMB_CHANNEL_PACKET_FAIL
author: windows-driver-content
description: The VmbChannelPacketFail function fails a packet during packet processing due to an unrecoverable error. This function stops the queue.
tech.root: netvista
ms.assetid: 00f1f4c0-60d4-46c9-b8c4-038e19cf5658
ms.author: windowsdriverdev
ms.date: 05/21/2018
ms.topic: callback
ms.prod: windows-hardware
ms.technology: windows-devices
req.header: vmbuskernelmodeclientlibapi.h
req.include-header:
req.target-type:
req.target-min-winverclnt: Windows 10, version 1803
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
-	vmbuskernelmodeclientlibapi.h
api_name: 
-	FN_VMB_CHANNEL_PACKET_FAIL
product:
-	Windows
targetos: Windows
---

# FN_VMB_CHANNEL_PACKET_FAIL callback function

## -description

<p class="CCE_Message">[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.]

The <b>VmbChannelPacketFail</b>  function fails a packet during packet processing due to an unrecoverable error. This function stops the queue.  

## -prototype

```
//Declaration

FN_VMB_CHANNEL_PACKET_FAIL FnVmbChannelPacketFail; 

// Definition

VOID FnVmbChannelPacketFail 
(
	VMBPACKETCOMPLETION PacketCompletionContext
)
{...}

```

## -parameters

### -param PacketCompletionContext

A  handle that identifies the incoming packet and is used to refer to the packet
once processing is finished. 

## -returns

This function does not return a value.

## -remarks

Call this function for packets presented to the server endpoint which seem malformed, to
the extent that channel processing should cease.

> [!IMPORTANT]
> This function is called through the VMBus Kernel Mode Client Library (KMCL) interface, provided by the Vmbkmcl.sys bus driver. This is a client function accessed from the [**KMCL_CLIENT_INTERFACE_V1**](ns-vmbuskernelmodeclientlibapi-_kmcl_client_interface_v1.md) structure. 
>
> For more information, see the Remarks section of the [**KMCL_CLIENT_INTERFACE_V1**](ns-vmbuskernelmodeclientlibapi-_kmcl_client_interface_v1.md).

## -see-also
