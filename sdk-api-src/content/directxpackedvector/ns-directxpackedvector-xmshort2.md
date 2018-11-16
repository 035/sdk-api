---
UID: NS:directxpackedvector.XMSHORT2
title: XMSHORT2
author: windows-sdk-content
description: Describes a 2D vector consisting of 16-bit signed and normalized integer components.
old-location: dxmath\xmshort2.htm
tech.root: dxmath
ms.assetid: T:Microsoft.directx_sdk.reference.XMSHORT2
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: XMSHORT2, XMSHORT2 structure [DirectX Math Support APIs], directxpackedvector/XMSHORT2, dxmath.xmshort2
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: directxpackedvector.h
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
 - DirectXPackedVector.h
api_name:
 - XMSHORT2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMSHORT2 structure


## -description


Describes a 2D vector consisting of 16-bit signed and normalized integer components.
    

For a list of additional functionality such as constructors and operators that are available
	using <code>XMSHORT2</code> when you are programming in C++, see <a href="https://msdn.microsoft.com/cc0db281-e304-408a-8b3d-2d520bfa283e">XMSHORT2 Extensions</a>.
<div class="alert"><b>Note</b>  See <a href="https://msdn.microsoft.com/31512657-c413-9e6e-e343-1ea677a02b8c">DirectXMath Library Type
	Equivalences</a> for information about equivalent <a href="https://msdn.microsoft.com/993fc7e4-4752-4bce-82d0-0a034fdc69c0">D3DDECLTYPE</a>, <a href="https://msdn.microsoft.com/a222e3bb-310c-4019-93ee-6a2da2a46ded">D3DFORMAT</a>, and <a href="https://msdn.microsoft.com/dce61bc4-4ed5-4e64-84e8-6db88025e5c2">DXGI_FORMAT</a> objects.
    </div><div> </div>

## -struct-fields




### -field x

Signed integer in the range [-32767, 32767] describing the x-coordinate
		    of the vector.
		


### -field y

Signed integer in the range [-32767, 32767] describing the y-coordinate
		    of the vector.
		


### -field v

 




## -remarks



The components are normalized when this structure is loaded into an <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a> using <a href="https://msdn.microsoft.com/70a53296-31be-48df-9f96-22d3041008f4">XMLoadShort2</a>. Each component will be divided by 32767.0f.
	

<b>Namespace:</b> Use DirectX::PackedVector

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/58acb05d-e79b-8f42-4cf4-76ae57929739">DirectXMath Library Structures</a>



<a href="https://msdn.microsoft.com/cc0db281-e304-408a-8b3d-2d520bfa283e">XMSHORT2 Extensions</a>
 

 

