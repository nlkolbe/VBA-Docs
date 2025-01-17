---
title: Shape.SetCaption method (Publisher)
ms.prod: publisher
ms.assetid: dd3ca08b-06c7-4a12-b51c-5d76ce1601b5
ms.date: 06/08/2017
localization_priority: Normal
---


# Shape.SetCaption method (Publisher)

Sets the caption style for the shape.


## Syntax

_expression_.**SetCaption**(**_Style_**)

_expression_ A variable that represents a **[Shape](Publisher.Shape.md)** object.


## Parameters



|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
|Style|Required| **CaptionStyle**|Specifies the style of the caption.|

## Return value

 **SHAPE**


## Remarks

This method works only if  `Shape.Type = pbPicture`.

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]