---
UID: The unique id of the API.
title: The title of the API.
author: Authoring type of the API(ie windows-driver-content)
description: Description of API
old-location: 
old-project: 
ms.assetid: The MSDN ID of the API
ms.author: The Author of the API
ms.date: The date of API publishing
ms.keywords: 
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: The topic type of the API (ie enum)
req.header: The main header of the API
req.include-header: The included headers of the API
req.target-type: 
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
---

# EngSort function


## -description


The <b>EngSort</b> function performs a quick-sort on the specified list.


## -parameters




### -param pjBuf [in, out]

Pointer to the data array to be sorted.


### -param c [in]

Specifies the size, in bytes, of each element in <i>pjBuf</i>.


### -param cjElem [in]

Specifies the number of elements in <i>pjBuf</i> to be sorted.


### -param pfnComp [in]

Pointer to a function that implements the element comparison to be used for the sort.


## -returns



None




## -remarks



<b>EngSort</b> implements a quick-sort algorithm to sort <i>cjElem</i> elements in <i>pjBuf</i>, where each element is of size <i>c</i>. The sorted elements are returned in <i>pjBuf</i>; that is, the original contents of the buffer are overwritten with the sorted results.

The basis for comparing two elements is defined in the function that <i>pfnComp </i>points to. This function is prototyped as follows:

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>int (__cdecl *SORTCOMP)(const void *pv1, const void *pv2);</pre>
</td>
</tr>
</table></span></div>
where <i>pv1</i> and <i>pv2</i> point to the two elements to be compared. The return value is the result of the comparison defined as follows:

<table>
<tr>
<th>Return Value</th>
<th>Meaning</th>
</tr>
<tr>
<td>
Negative integer

</td>
<td>
<i>*pv1</i> &lt; <i>*pv2</i>

</td>
</tr>
<tr>
<td>
Zero

</td>
<td>
<i>*pv1</i> == <i>*pv2</i>

</td>
</tr>
<tr>
<td>
Positive integer

</td>
<td>
<i>*pv1</i> &gt; <i>*pv2</i>

</td>
</tr>
</table>
 

The array is sorted in increasing order, which is defined by the <i>pfnComp</i> parameter.



