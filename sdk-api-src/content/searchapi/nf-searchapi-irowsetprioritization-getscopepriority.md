---
UID: NF:searchapi.IRowsetPrioritization.GetScopePriority
title: IRowsetPrioritization::GetScopePriority
author: windows-sdk-content
description: Retrieves the current indexer prioritization level for the scope specified by this query.
old-location: search\_search_IRowsetPrioritization_GetScopePriority.htm
tech.root: search
ms.assetid: VS|SEARCH|~\search\wds3x\reference\ifaces\querying\irowsetprioritization\getscopepriority.htm
ms.author: windowssdkdev
ms.date: 09/27/2018
ms.keywords: GetScopePriority, GetScopePriority method [search], GetScopePriority method [search],IRowsetPrioritization interface, IRowsetPrioritization interface [search],GetScopePriority method, IRowsetPrioritization.GetScopePriority, IRowsetPrioritization::GetScopePriority, _search_IRowsetPrioritization_GetScopePriority, search._search_IRowsetPrioritization_GetScopePriority, searchapi/IRowsetPrioritization::GetScopePriority
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: searchapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Searchquery.idl
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
 - Searchapi.h
api_name:
 - IRowsetPrioritization.GetScopePriority
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRowsetPrioritization::GetScopePriority


## -description


Retrieves the current indexer prioritization level for the scope specified by this query.

        


## -parameters




### -param priority [out]

Type: <b><a href="https://msdn.microsoft.com/d172ae7f-a495-4ea4-9d7d-ca8065f8d3cb">PRIORITY_LEVEL</a>*</b>

The current indexer prioritization level as the <a href="https://msdn.microsoft.com/d172ae7f-a495-4ea4-9d7d-ca8065f8d3cb">PRIORITY_LEVEL</a> enumeration.
        


### -param scopeStatisticsEventFrequency [out]

Type: <b>DWORD*</b>

The occurrence interval of the scope statistics event when there are outstanding documents to be indexed within the query scopes.
        


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The SearchEvents code sample, available on <a href="http://go.microsoft.com/fwlink/p/?linkid=155654">Code Gallery</a> and the <a href="http://go.microsoft.com/fwlink/p/?linkid=129787">Windows 7 SDK</a>, demonstrates how to prioritize indexing events.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/df16492c-e8f9-4d01-a8ad-cd76ea6bbc73">IRowsetEvents</a>



<a href="https://msdn.microsoft.com/82dce1fa-9bc5-4744-966e-1e7aa6fc3e05">IRowsetPrioritization</a>



<a href="https://msdn.microsoft.com/6cdfb7d3-f849-432c-960f-912e5024c583">Indexing Prioritization and Rowset Events in Windows 7</a>



<a href="https://msdn.microsoft.com/554d405e-c117-4597-9612-20cd6088ebef">PRIORITIZE_FLAGS</a>



<a href="https://msdn.microsoft.com/d172ae7f-a495-4ea4-9d7d-ca8065f8d3cb">PRIORITY_LEVEL</a>



<a href="https://msdn.microsoft.com/2df331c6-9048-4720-b582-0025461134c1">ROWSETEVENT_ITEMSTATE</a>



<a href="https://msdn.microsoft.com/c9fb74f6-8aed-4450-9bc4-d9f5c3e835a4">ROWSETEVENT_TYPE</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/71aa0ad6-ef34-47ee-945f-04bda20bf8a4">Rowset Properties</a>
 

 

