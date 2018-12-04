---
UID: NF:structuredquerycondition.ICondition.Clone
title: ICondition::Clone
author: windows-sdk-content
description: Creates a deep copy of this ICondition object.
old-location: search\_search_ICondition_Clone.htm
tech.root: search
ms.assetid: VS|search|~\search\wds3x\reference\ifaces\querying\icondition\clone.htm
ms.author: windowssdkdev
ms.date: 11/16/2018
ms.keywords: Clone, Clone method [search], Clone method [search],ICondition interface, ICondition interface [search],Clone method, ICondition.Clone, ICondition::Clone, _search_ICondition_Clone, search._search_ICondition_Clone, structuredquerycondition/ICondition::Clone
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: structuredquerycondition.h
req.include-header: Structuredquery.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 with SP1 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Structuredquery.idl
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
 - COM
api_location:
 - structuredquerycondition.h
api_name:
 - ICondition.Clone
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# ICondition::Clone


## -description


Creates a deep copy of this <a href="https://msdn.microsoft.com/7b880393-699d-438d-8d45-08fffc9d482f">ICondition</a> object.


## -parameters




### -param ppc [out, retval]

Type: <b><a href="https://msdn.microsoft.com/7b880393-699d-438d-8d45-08fffc9d482f">ICondition</a>**</b>

Receives a pointer to the clone of this <a href="https://msdn.microsoft.com/7b880393-699d-438d-8d45-08fffc9d482f">ICondition</a>.
            


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Because there are no methods for modifying an <a href="https://msdn.microsoft.com/7b880393-699d-438d-8d45-08fffc9d482f">ICondition</a>, there are few occasions when this method is necessary. In many cases it is adequate to call the <a href="_com_IUnknown_QueryInterface">IUnknown::QueryInterface</a> method on the <b>ICondition</b> to obtain an additional reference to the same object.
      




## -see-also




<a href="https://msdn.microsoft.com/d1ec553d-f9fb-4039-9121-0f57bac15345">CONDITION_OPERATION</a>



<a href="https://msdn.microsoft.com/921cdcb0-2915-4bbe-af4b-3f62c3867ea4">CONDITION_TYPE</a>



<a href="https://msdn.microsoft.com/7b880393-699d-438d-8d45-08fffc9d482f">ICondition</a>



<a href="https://msdn.microsoft.com/32c68ff7-f0f3-40eb-801a-c5c21ec496fa">ICondition2</a>



<b>Reference</b>
 

 

