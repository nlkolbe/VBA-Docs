---
title: Printer.PaperOrientation property (Publisher)
keywords: vbapb10.chm8978440
f1_keywords:
- vbapb10.chm8978440
ms.prod: publisher
api_name:
- Publisher.Printer.PaperOrientation
ms.assetid: f57986b6-e6c4-7a47-af93-56036d667240
ms.date: 06/08/2017
localization_priority: Normal
---


# Printer.PaperOrientation property (Publisher)

Gets or sets page orientation (landscape or portrait) for the printer. Read/write.


## Syntax

_expression_.**PaperOrientation**

_expression_ A variable that represents a **[Printer](Publisher.Printer.md)** object.


## Return value

PbOrientationType


## Remarks

Possible values for  **PaperOrientation** are **pbOrientationLandscape** (2) and **pbOrientationPortrait** (1).

The  **PaperOrientation** property setting corresponds to the **Orientation** setting on the **Publication and Paper Settings** tab of the **Print Setup** dialog box (**File** menu) in the Microsoft Publisher user interface.

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]