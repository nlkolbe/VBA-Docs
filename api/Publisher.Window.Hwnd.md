---
title: Window.Hwnd property (Publisher)
keywords: vbapb10.chm262161
f1_keywords:
- vbapb10.chm262161
ms.prod: publisher
api_name:
- Publisher.Window.Hwnd
ms.assetid: e0fe9b33-0839-a2a5-f939-9906e46f9632
ms.date: 06/08/2017
localization_priority: Normal
---


# Window.Hwnd property (Publisher)

Returns a  **Long** indicating the handle to the Microsoft Publisher application window. Read-only.


## Syntax

_expression_.**Hwnd**

_expression_ A variable that represents a **[Window](Publisher.Window.md)** object.


## Return value

Long


## Example

The following example displays the handle to the Publisher application window.


```vb
MsgBox "The handle to the Publisher application window is " & _ 
 Application.ActiveWindow.Hwnd
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]