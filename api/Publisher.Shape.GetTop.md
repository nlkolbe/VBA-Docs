---
title: Shape.GetTop method (Publisher)
keywords: vbapb10.chm2228247
f1_keywords:
- vbapb10.chm2228247
ms.prod: publisher
api_name:
- Publisher.Shape.GetTop
ms.assetid: 65421a42-a16a-2c9d-c510-f1c6066ae0bb
ms.date: 06/08/2017
localization_priority: Normal
---


# Shape.GetTop method (Publisher)

Returns the distance of the shape's or shape range's top edge from the top edge of the leftmost page in the current view as a  **Single** in the specified units.


## Syntax

_expression_.**GetTop**(**_Unit_**)

_expression_ A variable that represents a **[Shape](Publisher.Shape.md)** object.


## Parameters



|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
|Unit|Required| **PbUnitType**|The units in which to return the distance.|

## Return value

Single


## Remarks

The Unit parameter can be one of the  **[PbUnitType](Publisher.PbUnitType.md)** constants declared in the Microsoft Publisher type library.

Use the  **[GetLeft](Publisher.Shape.GetLeft.md)** method to return the distance of a shape's or shape range's left edge from the left edge of the leftmost page in the current view.


## Example

The following example displays the distances from the left and top edges of the leftmost page to the left and top edges of shape range consisting of all the shapes on the first page. The distances are expressed in inches (to the nearest hundredth).


```vb
With ActiveDocument.Pages(1).Shapes.Range 
 MsgBox "Distance from left: " _ 
 & Format(.GetLeft(Unit:=pbUnitInch), "0.00") _ 
 & " in" & vbCr _ 
 & "Distance from top: " _ 
 & Format(.GetTop(Unit:=pbUnitInch), "0.00") _ 
 & " in" 
End With
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]