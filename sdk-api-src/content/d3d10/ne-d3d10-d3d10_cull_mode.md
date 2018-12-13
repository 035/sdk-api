---
UID: NE:d3d10.D3D10_CULL_MODE
title: D3D10_CULL_MODE
author: windows-sdk-content
description: Indicates triangles facing a particular direction are not drawn.
old-location: direct3d10\d3d10_cull_mode.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\d3d10_cull_mode.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 2117693b-8d7e-4cd9-dfee-29b015d206b8, D3D10_CULL_BACK, D3D10_CULL_FRONT, D3D10_CULL_MODE, D3D10_CULL_MODE enumeration [Direct3D 10], D3D10_CULL_NONE, d3d10/D3D10_CULL_BACK, d3d10/D3D10_CULL_FRONT, d3d10/D3D10_CULL_MODE, d3d10/D3D10_CULL_NONE, direct3d10.d3d10_cull_mode
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
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
 - D3D10_CULL_MODE
product: Windows
targetos: Windows
req.typenames: D3D10_CULL_MODE
req.redist: 
---

# D3D10_CULL_MODE enumeration


## -description


Indicates triangles facing a particular direction are not drawn.


## -enum-fields




### -field D3D10_CULL_NONE

Always draw all triangles.


### -field D3D10_CULL_FRONT

Do not draw triangles that are front-facing.


### -field D3D10_CULL_BACK

Do not draw triangles that are back-facing.


## -remarks



This enumeration is part of a rasterizer-state object description (see <a href="https://msdn.microsoft.com/ae4bb4c4-35a8-43c3-bfa5-f57b44bc367e">D3D10_RASTERIZER_DESC</a>).




## -see-also




<a href="https://msdn.microsoft.com/3d1541bf-75d8-459d-a912-4068e9a0a9e4">Core Enumerations</a>
 

 

