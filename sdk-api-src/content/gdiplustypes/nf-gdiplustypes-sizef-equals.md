---
UID: NF:gdiplustypes.SizeF.Equals
title: SizeF::Equals
author: windows-sdk-content
description: The SizeF::Equals method determines whether two SizeF objects are equal.
old-location: gdiplus\_gdiplus_CLASS_SizeF_Equals_sz_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\sizefclass\sizefmethods\equals_12sz.htm
ms.author: windowssdkdev
ms.date: 10/19/2018
ms.keywords: Equals, Equals method [GDI+], Equals method [GDI+],SizeF class, SizeF class [GDI+],Equals method, SizeF.Equals, SizeF::Equals, _gdiplus_CLASS_SizeF_Equals_sz_, gdiplus._gdiplus_CLASS_SizeF_Equals_sz_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplustypes.h
req.include-header: Gdiplus.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Gdiplus.dll
api_name:
 - SizeF.Equals
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# SizeF::Equals


## -description


The <b>SizeF::Equals</b> method determines whether two 
			<a href="https://msdn.microsoft.com/b40ade07-f89e-44ba-9185-9aec01f1051f">SizeF</a> objects are equal.


## -parameters




### -param sz [in, ref]

Type: <b>const <a href="https://msdn.microsoft.com/b40ade07-f89e-44ba-9185-9aec01f1051f">SizeF</a></b>

Reference to a 
					<a href="https://msdn.microsoft.com/b40ade07-f89e-44ba-9185-9aec01f1051f">SizeF</a> object that is compared to this 
					<b>SizeF</b> object. 


## -returns



Type: <strong>Type: <b>BOOL</b>
</strong>

If the 
						<b>Width</b> and 
						<b>Height</b> data members of the two 
						<a href="https://msdn.microsoft.com/b40ade07-f89e-44ba-9185-9aec01f1051f">SizeF</a> objects are equal, this method returns <b>TRUE</b>; otherwise, it returns <b>FALSE</b>.




## -remarks



Two 
				<a href="https://msdn.microsoft.com/b40ade07-f89e-44ba-9185-9aec01f1051f">SizeF</a> objects are defined as equal if the 
				<b>Width</b> and 
				<b>Height</b> data members are equal.


#### Examples




```cpp
RectF rect(50.0f, 30.0f, 200.0f, 100.0f);
SizeF desiredSizeF(200.0f, 100.0f);
SizeF rectSizeF;

// Get the size of the rectangle.
rect.GetSize(&rectSizeF);

if(rectSizeF.Equals(desiredSizeF))
{
   // The rectangle has the wanted size.
} 
```





## -see-also




<a href="https://msdn.microsoft.com/6821442b-d352-48cb-a48a-839105a8c36a">RectF</a>



<a href="https://msdn.microsoft.com/8e3f7ddd-cac4-4e81-9764-40167ef7d9ef">Size Constructors</a>



<a href="https://msdn.microsoft.com/b40ade07-f89e-44ba-9185-9aec01f1051f">SizeF</a>
 

 

