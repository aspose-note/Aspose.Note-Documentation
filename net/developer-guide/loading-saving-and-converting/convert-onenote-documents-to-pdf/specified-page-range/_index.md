---
title: Converting a Specified Page Range of OneNote to PDF
type: docs
weight: 30
url: /net/convert-onenote-documents-to-pdf-format/specified-page-range/
---

The following code example demonstrates how to convert a OneNote into a PDF document with a specified page range as provided by the PdfSaveOptions class. It sets the PageIndex and PageCount properties.

{{< highlight csharp >}}
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions();

// Set page index
opts.PageIndex = 0;

// Set page count
opts.PageCount = 1;

dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";

// Save the document as PDF
oneFile.Save(dataDir, opts);
{{< /highlight >}}