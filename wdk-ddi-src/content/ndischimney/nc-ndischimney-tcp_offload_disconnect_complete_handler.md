---
UID: NC:ndischimney.TCP_OFFLOAD_DISCONNECT_COMPLETE_HANDLER
title: TCP_OFFLOAD_DISCONNECT_COMPLETE_HANDLER
author: windows-driver-content
description: NDIS calls a protocol driver's or intermediate driver's ProtocolTcpOffloadDisconnectComplete function to complete a disconnect operation that the driver previously initiated by calling the NdisOffloadTcpDisconnect function.
old-location: netvista\protocoltcpoffloaddisconnectcomplete.htm
tech.root: netvista
ms.assetid: 56244148-638f-4d93-82a6-2cced9744046
ms.author: windowsdriverdev
ms.date: 5/2/2018
ms.keywords: ProtocolTcpOffloadDisconnectComplete, ProtocolTcpOffloadDisconnectComplete callback function [Network Drivers Starting with Windows Vista], TCP_OFFLOAD_DISCONNECT_COMPLETE_HANDLER, TCP_OFFLOAD_DISCONNECT_COMPLETE_HANDLER callback, ndischimney/ProtocolTcpOffloadDisconnectComplete, netvista.protocoltcpoffloaddisconnectcomplete, tcp_chim_protocol_func_fadc0ea9-acd8-489d-886c-213b909d93b3.xml
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: ndischimney.h
req.include-header: Ndischimney.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	UserDefined
api_location:
-	Ndischimney.h
api_name:
-	ProtocolTcpOffloadDisconnectComplete
product:
- Windows
targetos: Windows
req.typenames: 
---

# TCP_OFFLOAD_DISCONNECT_COMPLETE_HANDLER callback function


## -description


<p class="CCE_Message">[The TCP chimney offload feature is deprecated and should not be used.]

NDIS calls a protocol driver's or intermediate driver's 
  <i>ProtocolTcpOffloadDisconnectComplete</i> function to complete a disconnect operation that the driver
  previously initiated by calling the 
  <a href="https://msdn.microsoft.com/f8abff30-b641-4581-8532-8292993ca9f6">
  NdisOffloadTcpDisconnect</a> function.


## -parameters




### -param ProtocolBindingContext [in]

A handle to a context area allocated by the protocol driver. The driver maintains the per binding
     context information in this context area. The driver supplied this handle to NDIS when the driver called
     the 
     <a href="https://msdn.microsoft.com/library/windows/hardware/ff563715">NdisOpenAdapterEx</a> function.


### -param NetBufferList [in]

When non-NULL, a pointer to a single 
     <a href="https://msdn.microsoft.com/library/windows/hardware/ff568388">NET_BUFFER_LIST</a> structure. The driver
     supplied this pointer as an input parameter in a previous call to the 
     <a href="https://msdn.microsoft.com/f8abff30-b641-4581-8532-8292993ca9f6">
     NdisOffloadTcpDisconnect</a> function.


## -returns



None




## -remarks



In response to an underlying driver's or offload target's call to the 
    <a href="https://msdn.microsoft.com/e862d9fe-a60c-4397-95ce-62aa1ef17eae">
    NdisTcpOffloadDisconnectComplete</a> function, NDIS calls the overlying protocol driver's or
    intermediate driver's 
    <i>ProtocolTcpOffloadDisconnectComplete</i> function.

To propagate the completion of the disconnect operation to the overlying driver, the intermediate
    driver calls the 
    <b>NdisOffloadTcpDisconnectComplete</b> function, passing in the following:

<ul>
<li>
A 
      <i>ProtocolBindingContext</i>, which is a handle that uniquely identifies the intermediate driver.

</li>
<li>
The same PNET_BUFFER_LIST pointer that NDIS passed to the intermediate driver's 
      <i>ProtocolTcpOffloadDisconnectComplete</i> function.

</li>
</ul>
In response, NDIS calls the overlying driver's 
    <i>ProtocolTcpOffloadDisconnectComplete</i> function, passing a 
    <i>ProtocolBindingContext</i> handle and the PNET_BUFFER_LIST pointer passed by the intermediate driver to
    the 
    <b>NdisOffloadTcpDisconnectComplete</b> function.

Before returning, the 
    <i>ProtocolTcpOffloadDisconnectComplete</i> function should deallocate the memory for any context that it
    created for the NET_BUFFER_LIST structure that was passed to the function.

Note that, if an intermediate driver exports more than one interface to overlying protocols, it must
    determine which protocol should receive the completion of the disconnect. To make this determination, the
    intermediate driver uses information that it stored in the 
    <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff568388">
    NET_BUFFER_LIST_CONTEXT</a> structure, which is associated with the NET_BUFFER_LIST structure.




## -see-also




<a href="https://msdn.microsoft.com/f8be12a9-c2c0-4a22-8a57-58c8b27ef69e">
   MiniportTcpOffloadDisconnect</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff568388">NET_BUFFER_LIST</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff563696">NdisOffloadTcpDisconnect</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff563715">NdisOpenAdapterEx</a>



<a href="https://msdn.microsoft.com/e862d9fe-a60c-4397-95ce-62aa1ef17eae">
   NdisTcpOffloadDisconnectComplete</a>
 

 

