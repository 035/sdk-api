---
UID: NS:d3d10.D3D10_COUNTER_INFO
title: D3D10_COUNTER_INFO
author: windows-sdk-content
description: Information about the video card's performance counter capabilities.
old-location: direct3d10\d3d10_counter_info.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\d3d10_counter_info.htm
ms.author: windowssdkdev
ms.date: 09/26/2018
ms.keywords: 556a7645-8a0b-b615-840b-b33669862365, D3D10_COUNTER_INFO, D3D10_COUNTER_INFO structure [Direct3D 10], d3d10/D3D10_COUNTER_INFO, direct3d10.d3d10_counter_info
ms.prod: windows
ms.technology: windows-sdk
ms.topic: struct
req.header: d3d10.h
req.include-header: 
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
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - D3D10.h
api_name:
 - D3D10_COUNTER_INFO
product: Windows
targetos: Windows
req.typenames: D3D10_COUNTER_INFO
req.redist: 
---

# D3D10_COUNTER_INFO structure


## -description


Information about the video card's performance counter capabilities.


## -struct-fields




### -field LastDeviceDependentCounter

Type: <b><a href="https://msdn.microsoft.com/b4c63ba3-29cf-4fb9-903f-28ac7750f9b6">D3D10_COUNTER</a></b>

Largest device-dependent counter ID that the device supports. If none are supported, this value will be 0. Otherwise it will be greater than or equal to D3D10_COUNTER_DEVICE_DEPENDENT_0. See <a href="https://msdn.microsoft.com/b4c63ba3-29cf-4fb9-903f-28ac7750f9b6">D3D10_COUNTER</a>.


### -field NumSimultaneousCounters

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Number of counters that can be simultaneously supported.


### -field NumDetectableParallelUnits

Type: <b>UINT8</b>

Number of detectable parallel units that the counter is able to discern. Values are 1 ~ 4. Use NumDetectableParallelUnits to interpret the values of the VERTEX_PROCESSING, GEOMETRY_PROCESSING, PIXEL_PROCESSING, and OTHER_GPU_PROCESSING counters. See <a href="https://msdn.microsoft.com/f8993ac8-3632-48d0-a583-08f117e8f587">ID3D10Asynchronous::GetData</a> for an equation.


## -remarks



This structure is returned by <a href="https://msdn.microsoft.com/dfa4cc61-2c1d-45a7-839c-f7df64d488ac">ID3D10Device::CheckCounterInfo</a>.




## -see-also




<a href="https://msdn.microsoft.com/84769515-3f3b-4464-9620-7b806bf905b3">Core Structures</a>
 

 

