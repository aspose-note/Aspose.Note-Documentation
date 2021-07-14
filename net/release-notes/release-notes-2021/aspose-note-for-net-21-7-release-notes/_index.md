---
title: Aspose.Note for .NET 21.7 Release Notes
type: docs
weight: 37
url: /net/aspose-note-for-net-21-7-release-notes/
---

{{% alert color="primary" %}} 

This page contains release notes information for [Aspose.Note for .NET 21.7](https://downloads.aspose.com/note/net/new-releases/aspose.note-for-.net-21.7/).

{{% /alert %}} 
## **Major Features**
- Specialized exception regarding OneNote 2007 format is not supported.
- Support of licenses with sha256
## **Features and Improvements**

|**Key**|**Summary**|**Category**|
| :- | :- | :- |
|NOTENET-3239|HyperLink Address is empty despite there is a hyperlink address in the one note file|Bug|
|NOTENET-3317|Exception "Not enough stream data" when opening password protected documents|Bug|
|NOTENET-3321|Add support of sha256 hashes to license validation algorithm|Feature|
|NOTENET-3318|Add special exception that OneNote 2007 format is not supported.|Feature|

## **Public API and Backward Incompatible Changes**

|**The following public constants were added:**|**Description**|
| :- | :- |
|Aspose.Note.FileFormat.OneNote2007|OneNote 2007 file format.|

|**The following public properties were removed:**|**Description**|
| :- | :- |
|Aspose.Note.Image.AlternativeText|Gets or sets an alternative text for the image.|
|Aspose.Note.RichText.DefaultStyle|Gets or sets the default style.|

|**The following public methods were removed:**|**Description**|
| :- | :- |
|Aspose.Note.CompositeNode.GetText|Get all text from the node.|
|Aspose.Note.Fonts.DocumentFontsSubsystem.#ctor(System.Drawing.FontFamily,System.Collections.Generic.Dictionary{System.String,System.String})|Initializes a new instance of the DocumentFontsSubsystem class.|
|Aspose.Note.Fonts.FontsSubsystem.#ctor(System.Drawing.FontFamily,System.Collections.Generic.Dictionary{System.String,System.String})|Initializes a new instance of the FontsSubsystem class. |
