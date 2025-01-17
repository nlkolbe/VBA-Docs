---
title: MasterPages.Add method (Publisher)
keywords: vbapb10.chm589828
f1_keywords:
- vbapb10.chm589828
ms.prod: publisher
api_name:
- Publisher.MasterPages.Add
ms.assetid: af237acb-9e4c-f9d8-685c-c86d58e9ee01
ms.date: 06/08/2017
localization_priority: Normal
---


# MasterPages.Add method (Publisher)

Adds a new  **Page** object to the specified **MasterPages** object and returns the new **Page** object.


## Syntax

_expression_.**Add** (_IsTwoPageMaster_, _Abbreviation_, _Description_**)

_expression_ A variable that represents a **[MasterPages](Publisher.MasterPages.md)** object.


## Parameters



|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
|IsTwoPageMaster|Optional| **Boolean**| **True** if the master page will be part of a two page spread.|
|Abbreviation|Optional| **String**|The abbreviation, or short name, for the master page. An error occurs if this is not unique.|
|Description|Optional| **String**|The description for the master page.|

## Return value

Page


## Example

The following example adds a new master page to the active document.


```vb
ActiveDocument.MasterPages.Add _ 
 IsTwoPageMaster:=False, _ 
 Abbreviation:="X", _ 
 Description:="Master Page X" 

```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]