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

# IWMPStringCollection2 interface


## -description



The <b>IWMPStringCollection2</b> interface provides methods that supplement the <b>IWMPStringCollection</b> interface.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMPStringCollection2</b> interface inherits from <a href="https://msdn.microsoft.com/8cdabea9-7e37-4e63-9d6c-b6f63aa536ea">IWMPStringCollection</a>. <b>IWMPStringCollection2</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMPStringCollection2</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/62e31749-2640-4b65-a8ee-47f3d3dd5485">getAttributeCountByType</a>
</td>
<td align="left" width="63%">
Retrieves the number of attributes associated with the specified string collection item index, attribute name, and language.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1915d71f-aca3-4943-a4da-ed8f2fa3f46d">getItemInfo</a>
</td>
<td align="left" width="63%">
Retrieves the string corresponding to the specified string collection item index and name.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ff395caf-9b5a-41e0-94c6-4a5eb96281ca">getItemInfoByType</a>
</td>
<td align="left" width="63%">
Retrieves the value corresponding to the specified string collection item index, name, language, and attribute index.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/549fdee8-7cd4-4ceb-8ed1-0de467d6c348">isIdentical</a>
</td>
<td align="left" width="63%">
Retrieves a value indicating whether the supplied object is the same as the current one.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/8cdabea9-7e37-4e63-9d6c-b6f63aa536ea">IWMPStringCollection Interface</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/dn965732">Interfaces</a>
 

 

