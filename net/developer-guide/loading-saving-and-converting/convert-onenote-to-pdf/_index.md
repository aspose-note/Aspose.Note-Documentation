---
title: Convert OneNote to PDF using C#
linktitle: Convert OneNote to PDF
type: docs
weight: 30
url: /net/convert-onenote-to-pdf/
keywords: convert onenote to pdf, export onenote to pdf
description: Convert or export OneNote to PDF document using C# or .NET API.
aliases:
  - /net/convert-onenote-documents-to-pdf-and-other-formats/
  - /net/convert-onenote-documents-to-pdf-format/
---

{{% alert color="primary" %}} 

Please note that you cannot set values against the **Application** and **Producer** fields, because of Aspose Ltd. and Aspose.Note for .NET x.x will be displayed against these fields.

{{% /alert %}} 


Time to time it turns out to be useful to share just a piece of gathered notes without providing access to full notes or add notes as a part of another document.
One of the best ways to achieve this goal is to save OneNote to PDF. PDF documents are widely used as a standard format of exchanging documents between organizations, government sectors and individuals. It's a popular format so developers are often asked to convert Microsoft OneNote documents to PDF documents. For this purpose, Aspose.Note for .NET supports converting OneNote to PDF documents without using any other component.
Software to deal with PDF documents is available almost on all platforms.

Using Microsoft OneNote desktop app you can export your notes to PDF format:
1. Select pages you want to export by holding Ctrl + mouse right-click 
2. Choose File -> Export
3. Under 'Export Current' choose what to export
4. Under 'Select Format' choose option for pdf
5. Press export and specify destination file name

All selected content will be saved to specified file.


The second option provided by Microsoft OneNote is to install custom pdf printer like CutePDF/PDFCreator.
Using this option:
1. Select pages you want to export by holding Ctrl + mouse right-click 
2. Choose File -> Print
3. Select your pdf printer
4. Press 'Preferences' to review and change settings
5. Press 'Print' and specify destination file.


As you see both options provided by Microsoft OneNote lack of settings to tune saving.
Aspose.Note fills this gap and supports export to PDF with a set of useful settings.
Using latest version of Aspose.Note you can:
1. Specify any range of pages to be saved.
2. Specify settings for image compression.
3. Handle absent fonts.
4. Control how content is splitted to pdf pages.


Aspose.Note for .NET offers the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents a OneNote document. The Document class exposes the Save method that can be called to convert a OneNote document into a PDF document. The [PdfSaveOptions](https://apireference.aspose.com/note/net/aspose.note.saving/pdfsaveoptions) class allows to specify additional settings for saving operation.


## **Convert OneNote to PDF**
[Basic samples of how to convert OneNote to PDF](https://docs.aspose.com/note/net/convert-onenote-to-pdf/basic-samples/)
[Convert of OneNote to PDF with replacing of missing fonts](https://docs.aspose.com/note/net/convert-onenote-to-pdf/replacing-of-missing-fonts/)

