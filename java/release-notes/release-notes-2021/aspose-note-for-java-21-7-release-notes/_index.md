---
title: Aspose.Note for Java 21.7 Release Notes
type: docs
weight: 37
url: /java/aspose-note-for-java-21-7-release-notes/
---

{{% alert color="primary" %}} 

This page contains release notes information for [Aspose.Note for Java 21.7](https://downloads.aspose.com/note/java/new-releases/aspose.note-for-java-21.7/).

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
|com.aspose.note.FileFormat.OneNote2007|OneNote 2007 file format.|

|**The following public methods were removed:**|**Description**|
| :- | :- |
|com.aspose.note.CompositeNode.getText|Get all text from the node.|
|com.aspose.note.fonts.DocumentFontsSubsystem.#ctor(java.awt.Font,java.util.Map)|Initializes a new instance of the DocumentFontsSubsystem class.|
|com.aspose.note.fonts.DocumentFontsSubsystem.#ctor(java.awt.Font)|Initializes a new instance of the DocumentFontsSubsystem class.|
|com.aspose.note.fonts.FontsSubsystem.#ctor(java.awt.Font,java.util.Map)|Initializes a new instance of the FontsSubsystem class. |
|com.aspose.note.fonts.FontsSubsystem.#ctor(java.awt.Font)|Initializes a new instance of the FontsSubsystem class. |
|com.aspose.note.Image.getAlternativeText|Gets an alternative text for the image.|
|com.aspose.note.Image.setAlternativeText(java.lang.String)|Sets an alternative text for the image.|
|com.aspose.note.RichText.getDefaultStyle|Gets the default style.|
|com.aspose.note.RichText.setDefaultStyle(com.aspose.note.TextStyle)|Sets the default style.|
