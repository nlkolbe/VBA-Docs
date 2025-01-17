---
title: ShapeRange.Table property (Publisher)
keywords: vbapb10.chm2293864
f1_keywords:
- vbapb10.chm2293864
ms.prod: publisher
api_name:
- Publisher.ShapeRange.Table
ms.assetid: 68221d37-505a-4701-8c9d-b8e695c8eb8f
ms.date: 06/08/2017
localization_priority: Normal
---


# ShapeRange.Table property (Publisher)

Returns a  **Table** object that represents a table in Microsoft Publisher.


## Syntax

_expression_.**Table**

_expression_ A variable that represents a **[ShapeRange](Publisher.ShapeRange.md)** object.


## Example

The following example adds a 5x5 table on the first page of the active publication, and then selects the first column of the new table.


```vb
Sub NewTable() 
 With ActiveDocument.Pages(1).Shapes.AddTable(NumRows:=5, _ 
 NumColumns:=5, Left:=72, Top:=300, Width:=400, Height:=100) 
 .Table.Columns(3).Cells(3).Fill.ForeColor.RGB = RGB _ 
 (Red:=255, Green:=0, Blue:=0) 
 End With 
End Sub
```

The following example selects the specified table in the active publication. This example assumes that there is at least one shape on the first page of the active publication.




```vb
Sub SelectTable() 
 With ActiveDocument.Pages(1).Shapes(1) 
 If .Type = pbTable Then 
 .Table.Rows(3).Cells(3).Fill.ForeColor _ 
 .RGB = RGB(Red:=150, Green:=150, Blue:=150) 
 End If 
 End With 
End Sub
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]