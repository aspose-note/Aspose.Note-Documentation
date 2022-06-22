---
title: Import Pdf to OneNote
type: docs
weight: 30
url: /net/import/import-from-pdf/
keywords: import from pdf to onenote
description: Import from Pdf to OneNote using C# or .NET API.
---

Time to time is useful to import a piece of content from documents in other formats. One of the most popular formats is PDF. PDF is widely used as a standard format of exchanging documents between organizations, government sectors and in private.

If you need a good PDF  converter in OneNote then pay attention to our product. With our application, you can easily convert PDF to OneNote and vice versa.

Aspose.Note for .NET supports importing from PDF  without using any other component and provides a set of useful settings to accomplish this task. Using latest version of Aspose.Note you can:

1. Specify any range of pages in Pdf document to import.
2. Control how imported pages are merged to OneNote document.

It comes with the software library to help you convert and manage your PDF files into OneNote.

## **How to convert Pdf to OneNote**

The Import method exposed by the Aspose.Note API lets you import data from the document in Pdf format:

- Import(Stream, PdfImportOptions, MergeOptions)
- Import(string, PdfImportOptions, MergeOptions)


## **Import all data from a set of Pdf files**

You can import any data. It can be a text, an image, a table.
The sample below shows how to import all pages from a set of PDF files page by page.

{{< highlight csharp >}}
var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));

{{< /highlight >}}


## **Import every Pdf as single OneNote page**

Time to time it is useful to just import all data from Pdf file as a single page. It can be any small document of few pages size like report/invoice/etc.

The sample below shows how to import all data from a set of PDF documents while merging pages from every PDF document to a single OneNote page.

{{< highlight csharp >}}
var d = new Document();

var importOptions = new PdfImportOptions();
var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

d.Import(Path.Combine(dataDir, "sampleText.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleImage.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleTable.pdf"), importOptions, mergeOptions);

d.Save(Path.Combine(dataDir, "sample_SinglePageMerge.one"));

{{< /highlight >}}


## **Import all pages from Pdf and merge them using custom logic**

Sometimes it is necessary to merge Pdf files according to a certain rule or logic. 
In this case a simple merging will not help us and in order to achieve our goal it is necessary to write custom logic for selecting pages and merging them to OneNote document.

The sample below shows how to import all pages from PDF grouping every 5 pages to a single OneNote page.

{{< highlight csharp >}}
var d = new Document();

var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

IEnumerable<Page> pages = PdfImporter.Import(Path.Combine(dataDir, "SampleGrouping.pdf"));
while (pages.Any())
{
    d.Merge(pages.Take(5), mergeOptions);
    pages = pages.Skip(5);
}

d.Save(Path.Combine(dataDir, "sample_CustomMerge.one"));

{{< /highlight >}}
