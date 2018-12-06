---
UID: NF:structuredquery.IConditionFactory2.CreateLeaf
title: IConditionFactory2::CreateLeaf
author: windows-sdk-content
description: Creates a leaf condition node for any value. The returned object supports ICondition and ICondition2.
old-location: search\_search_IConditionFactory2_CreateLeaf.htm
tech.root: search
ms.assetid: VS|SEARCH|~\search\wds3x\reference\ifaces\querying\iconditionfactory\createleaf.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateLeaf, CreateLeaf method [search], CreateLeaf method [search],IConditionFactory2 interface, IConditionFactory2 interface [search],CreateLeaf method, IConditionFactory2.CreateLeaf, IConditionFactory2::CreateLeaf, _search_IConditionFactory2_CreateLeaf, search._search_IConditionFactory2_CreateLeaf, structuredquery/IConditionFactory2::CreateLeaf
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: structuredquery.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - IConditionFactory2.CreateLeaf
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IConditionFactory2::CreateLeaf


## -description


Creates a leaf condition node for any value. The returned object supports <a href="https://msdn.microsoft.com/7b880393-699d-438d-8d45-08fffc9d482f">ICondition</a> and <a href="https://msdn.microsoft.com/32c68ff7-f0f3-40eb-801a-c5c21ec496fa">ICondition2</a>.
        


## -parameters




### -param propkey [in]

Type: <b>REFPROPERTYKEY</b>

The name of the property of the leaf condition as a REFPROPERTYKEY. If the leaf has no particular property, use PKEY_Null.


### -param cop [in]

Type: <b><a href="https://msdn.microsoft.com/d1ec553d-f9fb-4039-9121-0f57bac15345">CONDITION_OPERATION</a></b>

A <a href="https://msdn.microsoft.com/d1ec553d-f9fb-4039-9121-0f57bac15345">CONDITION_OPERATION</a> enumeration. If the leaf has no particular operation, then use <i>COP_IMPLICIT</i>.


### -param propvar [in]

Type: <b>REFPROPERTYKEY</b>

The property value of the leaf condition as a REFPROPERTYKEY.


### -param pszSemanticType [in, optional]

Type: <b>LPCWSTR</b>

The name of a semantic type of the value, or <b>NULL</b> for a plain string. If the newly created leaf is an unresolved named entity, <i>pszSemanticType</i> should be the name of a semantic type, otherwise <b>NULL</b>.
            


### -param pszLocaleName [in, optional]

Type: <b>LPCWSTR</b>

The name of the locale to be compared, or <b>NULL</b> for an unspecified locale. If <i>propvar</i> does not contain a string value, then <i>pszLocaleName</i> should be LOCALE_NAME_USER_DEFAULT; otherwise, <i>pszLocaleName</i> should reflect the language the string. Alternatively, <i>pszLocaleName</i> could be  LOCALE_NAME_INVARIANT.
            


### -param pPropertyNameTerm [in, optional]

Type: <b><a href="https://msdn.microsoft.com/5fcc5c82-8d56-4495-8248-cf2fd19dd85a">IRichChunk</a>*</b>

A pointer to an <a href="https://msdn.microsoft.com/5fcc5c82-8d56-4495-8248-cf2fd19dd85a">IRichChunk</a> that identifies the range of the input string that repesents the property. It can be <b>NULL</b>.
            


### -param pOperationTerm [in, optional]

Type: <b><a href="https://msdn.microsoft.com/5fcc5c82-8d56-4495-8248-cf2fd19dd85a">IRichChunk</a>*</b>

A pointer to an <a href="https://msdn.microsoft.com/5fcc5c82-8d56-4495-8248-cf2fd19dd85a">IRichChunk</a> that identifies the range of the input string that repesents the operation. It can be <b>NULL</b>.
            


### -param pValueTerm [in, optional]

Type: <b><a href="https://msdn.microsoft.com/5fcc5c82-8d56-4495-8248-cf2fd19dd85a">IRichChunk</a>*</b>

A pointer to an <a href="https://msdn.microsoft.com/5fcc5c82-8d56-4495-8248-cf2fd19dd85a">IRichChunk</a> that identifies the range of the input string that repesents the value. It can be <b>NULL</b>.
            


### -param cco [in]

Type: <b><a href="https://msdn.microsoft.com/5fa88dc1-8ca3-4247-8bad-bba8be2ad734">CONDITION_CREATION_OPTIONS</a></b>

The condition creation operation of the leaf condition as the <a href="https://msdn.microsoft.com/5fa88dc1-8ca3-4247-8bad-bba8be2ad734">CONDITION_CREATION_OPTIONS</a> enumeration.


### -param riid [in]

Type: <b>REFIID</b>

The desired IID of the enumerating interface: either <a href="_com_IEnumUnknown">IEnumUnknown</a>, <a href="139e3c93-faef-4003-9079-e0e94494db3e">IEnumVARIANT</a>, or (for a negation condition) IID_ICondition.


### -param ppv [out]

Type: <b>void**</b>

Receives a pointer to zero or more <a href="https://msdn.microsoft.com/7b880393-699d-438d-8d45-08fffc9d482f">ICondition</a> and <a href="https://msdn.microsoft.com/32c68ff7-f0f3-40eb-801a-c5c21ec496fa">ICondition2</a> objects.


## -returns



This method does not return a value.




## -remarks



For default options, use the <i>CONDITION_CREATION_DEFAULT</i> flag.

 If the leaf condition was obtained by parsing a string, one or more of the parameters <i>pPropertyNameTerm</i>, <i>pOperationTerm </i> and <i>pValueTerm</i> may be represented by an <a href="https://msdn.microsoft.com/5fcc5c82-8d56-4495-8248-cf2fd19dd85a">IRichChunk</a> interface (obtained through the <a href="https://msdn.microsoft.com/9d169fb4-177f-42e6-a24c-bb0052d1d62b">ICondition::GetInputTerms</a> method). Otherwise all three parameters can be <b>NULL</b>. 

For more information about leaf node terms (property, value, and operation), see 
<a href="https://msdn.microsoft.com/9d169fb4-177f-42e6-a24c-bb0052d1d62b">ICondition::GetInputTerms</a>.

A virtual property has one or more metadata items in which the key is "MapsToRelation" and the value is a property name (which is one expansion of the property). For more information about metadata, see <a href="https://msdn.microsoft.com/b3322f0c-8929-4f0f-8d2d-44f063ff83db">MetaData</a>. 
     




## -see-also




<a href="https://msdn.microsoft.com/5fa88dc1-8ca3-4247-8bad-bba8be2ad734">CONDITION_CREATION_OPTIONS</a>



<a href="https://msdn.microsoft.com/d1ec553d-f9fb-4039-9121-0f57bac15345">CONDITION_OPERATION</a>



<a href="https://msdn.microsoft.com/921cdcb0-2915-4bbe-af4b-3f62c3867ea4">CONDITION_TYPE</a>



<a href="https://msdn.microsoft.com/7b880393-699d-438d-8d45-08fffc9d482f">ICondition</a>



<a href="https://msdn.microsoft.com/32c68ff7-f0f3-40eb-801a-c5c21ec496fa">ICondition2</a>



<a href="https://msdn.microsoft.com/c678fa37-8673-4da7-9c23-9a7f478dc1b0">IConditionFactory</a>



<a href="https://msdn.microsoft.com/5ac0acb1-67f0-43f0-b1c1-2d8cf682a277">IConditionFactory2</a>



<b>Reference</b>
 

 

