---
UID: NS:directxpackedvector.XMUSHORTN2
title: XMUSHORTN2
author: windows-sdk-content
description: A 2D vector for storing unsigned, normalized values as unsigned 16-bit integers, (type uint16_t).
old-location: dxmath\xmushortn2.htm
tech.root: dxmath
ms.assetid: T:Microsoft.directx_sdk.reference.XMUSHORTN2
ms.author: windowssdkdev
ms.date: 11/02/2018
ms.keywords: XMUSHORTN2, XMUSHORTN2 structure [DirectX Math Support APIs], directxpackedvector/XMUSHORTN2, dxmath.xmushortn2
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
 - XMUSHORTN2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMUSHORTN2 structure


## -description


A 2D vector for storing unsigned, normalized values as unsigned 16-bit integers, (type
	<code>uint16_t</code>).
    



For a list of more functionality such as constructors and operators that are available
	using <code>XMUSHORTN2</code> when you are programming in C++, see <a href="https://msdn.microsoft.com/b13018c2-cb31-45d6-ba42-f94945a0b63b">XMUSHORTN2 Extensions</a>.
<div class="alert"><b>Note</b>  See <a href="https://msdn.microsoft.com/31512657-c413-9e6e-e343-1ea677a02b8c">DirectXMath Library Type
	Equivalences</a> for information about equivalent <a href="https://msdn.microsoft.com/993fc7e4-4752-4bce-82d0-0a034fdc69c0">D3DDECLTYPE</a>, <a href="https://msdn.microsoft.com/a222e3bb-310c-4019-93ee-6a2da2a46ded">D3DFORMAT</a>, and <a href="https://msdn.microsoft.com/dce61bc4-4ed5-4e64-84e8-6db88025e5c2">DXGI_FORMAT</a> objects.
    </div><div> </div>

## -struct-fields




### -field x

Unsigned integer in the range [0, 65536] describing the x-coordinate
		    of the vector.
		


### -field y

Unsigned integer in the range [0, 65536] describing the y-coordinate
		    of the vector.
		


### -field v

 




## -remarks



Those <code>XMUSHORTN2</code> constructors using floating point arguments require normalized input,
	    which must be in the range of [0.0.-1.0].  During instantiation, data is
	    multiplied by 65535.0f, results are rounded, and then assigned to the appropriate
	    members of <code>XMUSHORTN2</code>.
	    
	

You can use <code>XMUSHORTN2</code> to load instances of <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a> from
	    normalized values by using <a href="https://msdn.microsoft.com/74cf23de-199a-48e6-81f1-b43762f103b4">XMLoadShortN4</a>, which divides each
	    component 65535.0f, rounds the result, and then assigns the components to an
	    <code>XMVECTOR</code> instance.
	

You can store <code>XMVECTOR</code> instances containing normalized values into <code>XMUSHORTN2</code>using <a href="https://msdn.microsoft.com/dd59f88a-520f-4028-9940-6c234057c6fa">XMStoreShortN4</a>, which multiplies each component by 65535.0f
	    and rounds the result before assigning the values to the appropriate <code>XMUSHORTN2</code> members.
	

<b>Namespace:</b> Use DirectX::PackedVector

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/58acb05d-e79b-8f42-4cf4-76ae57929739">DirectXMath Library Structures</a>



<a href="https://msdn.microsoft.com/b13018c2-cb31-45d6-ba42-f94945a0b63b">XMUSHORTN2 Extensions</a>
 

 

