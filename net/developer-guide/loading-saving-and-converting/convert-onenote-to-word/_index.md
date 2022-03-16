---
title: Convert OneNote to Word
type: docs
weight: 30
url: /net/convert-onenote-to-word/
keywords: convert onenote to word, export onenote to word
description: Convert or export OneNote to Word document using C# or .NET API.
---

Time to time it turns out to be useful to share just a piece of gathered notes without providing access to full notes or add notes as a part of another document.
One of the options to achieve this goal is to save OneNote to Word. Word documents are widely used as a standard format of exchanging documents between organizations, government sectors and individuals. It's a popular format so developers are often asked to convert Microsoft OneNote documents to Word documents.
Software to deal with Word documents is available almost on all platforms.

Using Microsoft OneNote desktop app you can export your notes to Word format:
1. Select pages you want to export by holding Ctrl + mouse right-click 
2. Choose File -> Export
3. Under 'Export Current' choose what to export
4. Under 'Select Format' choose option for Word format
5. Press export and specify destination file name

All selected content will be saved to specified file.


As you see Microsoft OneNote doesn't provide variety of settings to tune saving.

At the moment Aspose.Note cannot directly save Onenote to Word but you can use another Aspose products like Aspose.Words and Aspose.Pdf providing a set of useful settings to accomplish this task.
Using latest version of Aspose.Note you can:
1. Specify any range of pages to be saved.
2. Specify settings for image compression.
3. Handle absent fonts.
4. Control how content is splitted to pdf pages.

## **Convert OneNote to Word using Aspose.Words**

The sample below shows how to convert OneNote to Word using Aspose.Words.

{{< highlight csharp >}}
var one = new Document(...);

var stream = new MemoryStream();
one.Save(stream, SaveFormat.Pdf);

stream.Seek(0, SeekOrigin.Begin);

var word = new Aspose.Words.Document(stream);
word.Save("sample.docx");

{{< /highlight >}}


## **Convert OneNote to Word using Aspose.PDF**

The sample below shows how to convert OneNote to Word using Aspose.PDF.

{{< highlight csharp >}}
var one = new Document(...);

var stream = new MemoryStream();
one.Save(stream, SaveFormat.Pdf);

stream.Seek(0, SeekOrigin.Begin);

var pdf = new Aspose.Pdf.Document(stream);
pdf.Save("sample.docx", Aspose.Pdf.SaveFormat.DocX);

{{< /highlight >}}
