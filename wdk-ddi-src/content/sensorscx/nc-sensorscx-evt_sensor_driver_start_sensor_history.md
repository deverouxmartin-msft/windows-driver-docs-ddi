---
UID: NC:sensorscx.EVT_SENSOR_DRIVER_START_SENSOR_HISTORY
title: EVT_SENSOR_DRIVER_START_SENSOR_HISTORY
author: windows-driver-content
description: Starts recording history in the sensor.
ms.assetid: f2c80711-989b-48ff-a7f2-01635de2841d
ms.author: windowsdriverdev
ms.date: 
ms.topic: callback
ms.prod: windows-hardware
ms.technology: windows-devices
req.header: sensorscx.h
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
-	sensorscx.h
api_name: 
-	EVT_SENSOR_DRIVER_START_SENSOR_HISTORY
product:
- Windows
targetos: Windows
---

# EVT_SENSOR_DRIVER_START_SENSOR_HISTORY callback function

## -description

Starts recording history in the sensor.

## -prototype

```
//Declaration

EVT_SENSOR_DRIVER_START_SENSOR_HISTORY EvtSensorDriverStartSensorHistory; 

// Definition

NTSTATUS EvtSensorDriverStartSensorHistory 
(
	SENSOROBJECT Sensor
)
{...}

```

## -parameters

### -param Sensor

[in] A reference to a sensor object.

## -returns

Returns NTSTATUS.