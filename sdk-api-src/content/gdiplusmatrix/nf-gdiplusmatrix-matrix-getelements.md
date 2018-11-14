---
UID: NF:gdiplusmatrix.Matrix.GetElements
title: Matrix::GetElements
author: windows-sdk-content
description: The Matrix::GetElements method gets the elements of this matrix. The elements are placed in an array in the order m11, m12, m21, m22, m31, m32, where mij denotes the element in row i, column j.
old-location: gdiplus\_gdiplus_CLASS_Matrix_GetElements_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\matrixclass\matrixmethods\getelements.htm
ms.author: windowssdkdev
ms.date: 11/09/2018
ms.keywords: GetElements, GetElements method [GDI+], GetElements method [GDI+],Matrix class, Matrix class [GDI+],GetElements method, Matrix.GetElements, Matrix::GetElements, _gdiplus_CLASS_Matrix_GetElements_, gdiplus._gdiplus_CLASS_Matrix_GetElements_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusmatrix.h
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
 - Matrix.GetElements
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- COM
: 
- gdiplusmatrix.h
: 
- Matrix.GetElements
: 
req.product: GDI+ 1.0
---

# Matrix::GetElements


## -description


The <b>Matrix::GetElements</b> method gets the elements of this matrix. The elements are placed in an array in the order m11, m12, m21, m22, m31, m32, where mij denotes the element in row i, column j.


## -parameters




### -param m [out]

Type: <b>REAL*</b>

Pointer to an array that receives the matrix elements. The size of the array should be 6
					×<b>sizeof</b>(
					<b>REAL</b>). 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a></b>
</strong>

If the method succeeds, it returns OK, which is an element of the 
						<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/9f744c2a-f1f3-4a7e-ab0c-37aa1df01623">Global and Local Transformations</a>



<a href="https://msdn.microsoft.com/92b0d9db-3d4c-47b8-87cd-60d7b4323f0a">Matrix</a>



<a href="https://msdn.microsoft.com/62215ae0-b095-42b2-911c-aa7607a8b61a">Matrix Representation of Transformations</a>



<a href="https://msdn.microsoft.com/8b1cc844-eea9-46e2-bfdc-9fb1387a5da4">Matrix::SetElements</a>



<a href="https://msdn.microsoft.com/4acf3d70-f119-4a5b-a20d-8adea453556f">Transformations</a>
 

 

