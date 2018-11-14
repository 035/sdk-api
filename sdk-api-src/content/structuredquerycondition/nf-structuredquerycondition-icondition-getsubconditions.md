---
UID: NF:structuredquerycondition.ICondition.GetSubConditions
title: ICondition::GetSubConditions
author: windows-sdk-content
description: Retrieves a collection of the subconditions of the search condition node and the IID of the interface for enumerating the collection.
old-location: search\_search_ICondition_GetSubConditions.htm
tech.root: search
ms.assetid: VS|search|~\search\wds3x\reference\ifaces\querying\icondition\getsubconditions.htm
ms.author: windowssdkdev
ms.date: 09/27/2018
ms.keywords: GetSubConditions, GetSubConditions method [search], GetSubConditions method [search],ICondition interface, ICondition interface [search],GetSubConditions method, ICondition.GetSubConditions, ICondition::GetSubConditions, _search_ICondition_GetSubConditions, search._search_ICondition_GetSubConditions, structuredquerycondition/ICondition::GetSubConditions
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
 - ICondition.GetSubConditions
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
- apiref
: 
- COM
: 
- structuredquerycondition.h
: 
- ICondition.GetSubConditions
: 
---

# ICondition::GetSubConditions


## -description


Retrieves a collection of the subconditions of the search condition node and the IID of the interface for enumerating the collection.
        


## -parameters




### -param riid [in]

Type: <b>REFIID</b>

The desired IID of the enumerating interface: either IID_IEnumUnknown, IID_IEnumVARIANT or (for a negation condition) IID_ICondition.
            


### -param ppv [out, retval]

Type: <b>void**</b>

Receives a collection of zero or more <a href="https://msdn.microsoft.com/7b880393-699d-438d-8d45-08fffc9d482f">ICondition</a> objects. Each object is a subcondition of this condition node. If <i>riid</i> was IID_ICondition and this is a negation condition, this parameter receives the single subcondition.
            


## -returns



Type: <b>HRESULT</b>

Returns S_OK if successful, E_FAIL if this is a leaf node, or an error value otherwise.




## -remarks



The <i>riid</i> parameter must be the <b>GUID</b> of an <a href="_com_IEnumUnknown">IEnumUnknown</a> or <a href="139e3c93-faef-4003-9079-e0e94494db3e">IEnumVARIANT</a> interface or in the case of a negation node, IID_ICondition.

If the subcondition is a negation node, <i>ppv</i> is set to an enumeration of one element.

If the node is a conjunction or disjunction node, <i>ppv</i> is set to an enumeration of the subconditions.




## -see-also




<a href="https://msdn.microsoft.com/d1ec553d-f9fb-4039-9121-0f57bac15345">CONDITION_OPERATION</a>



<a href="https://msdn.microsoft.com/921cdcb0-2915-4bbe-af4b-3f62c3867ea4">CONDITION_TYPE</a>



<a href="https://msdn.microsoft.com/7b880393-699d-438d-8d45-08fffc9d482f">ICondition</a>



<a href="https://msdn.microsoft.com/32c68ff7-f0f3-40eb-801a-c5c21ec496fa">ICondition2</a>



<b>Reference</b>
 

 

