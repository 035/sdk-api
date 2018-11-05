---
UID: NF:structuredquery.ISchemaProvider.LookupAuthoredNamedEntity
title: ISchemaProvider::LookupAuthoredNamedEntity
author: windows-sdk-content
description: Finds named entities of a specified type in a tokenized string, and returns the value of the entity and the number of tokens the entity value occupies.
old-location: search\_search_ISchemaProvider_LookupAuthoredNamedEntity.htm
tech.root: search
ms.assetid: VS|search|~\search\wds3x\reference\ifaces\querying\ischemaprovider\lookupauthorednamedentity.htm
ms.author: windowssdkdev
ms.date: 09/27/2018
ms.keywords: ISchemaProvider interface [search],LookupAuthoredNamedEntity method, ISchemaProvider.LookupAuthoredNamedEntity, ISchemaProvider::LookupAuthoredNamedEntity, LookupAuthoredNamedEntity, LookupAuthoredNamedEntity method [search], LookupAuthoredNamedEntity method [search],ISchemaProvider interface, _search_ISchemaProvider_LookupAuthoredNamedEntity, search._search_ISchemaProvider_LookupAuthoredNamedEntity, structuredquery/ISchemaProvider::LookupAuthoredNamedEntity
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: structuredquery.h
req.include-header: 
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
 - Structuredquery.h
api_name:
 - ISchemaProvider.LookupAuthoredNamedEntity
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# ISchemaProvider::LookupAuthoredNamedEntity


## -description


Finds named entities of a specified type in a tokenized string, and returns the value of the entity and the number of tokens the entity value occupies. 


## -parameters




### -param pEntity [in]

Type: <b><a href="https://msdn.microsoft.com/856018d4-5e72-421e-9760-49f5d8d77e79">IEntity</a>*</b>

A pointer to an <a href="https://msdn.microsoft.com/856018d4-5e72-421e-9760-49f5d8d77e79">IEntity</a> object identifying the type of named entity to locate.


### -param pszInputString [in]

Type: <b>LPCWSTR</b>

An input string in which to search for named entity keywords.


### -param pTokenCollection [in]

Type: <b><a href="https://msdn.microsoft.com/e7f5b3ce-dae2-41ec-90ff-9ab49e0301bd">ITokenCollection</a>*</b>

A pointer to the tokenization of the string in the <i>pszInputString</i> parameter.


### -param cTokensBegin [in]

Type: <b>ULONG</b>

The zero-based position of a token in the <i>pTokenCollection</i> from which to start searching.


### -param pcTokensLength [out]

Type: <b>ULONG*</b>

Receives a pointer to the number of tokens covered by the named entity keyword that was found.


### -param ppszValue [out]

Type: <b>LPWSTR*</b>

Receives a pointer to the value of the named entity that was found, as a Unicode string. The caller must free the string by calling <a href="_com_CoTaskMemFree">CoTaskMemFree</a>. An <a href="https://msdn.microsoft.com/1e5dfef8-0f54-4302-97d8-bcbc0edbef03">INamedEntity</a> object can be obtained by calling the <a href="https://msdn.microsoft.com/aa1a5324-3c23-4e6c-9e97-1a08996a6093">GetNamedEntity</a> method of <i>pEntity</i> and passing the string that was received in this parameter.



## -returns



Type: <b>HRESULT</b>

Returns S_OK if the token sequence beginning at position <i>cTokensBegin</i> denotes a named entity of the specified (entity) type. If there is no such token sequence, returns S_FALSE.
                




## -remarks



The method finds only named entities authored with keywords in the schema, not named entities recognized by an <a href="https://msdn.microsoft.com/30fa2fb6-7dfd-41e1-ab4f-5fd80c8a81ec">IConditionGenerator</a> object.
            



