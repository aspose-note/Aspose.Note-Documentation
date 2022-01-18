---
title: Basic samples how to convert OneNote to PDF
type: docs
weight: 30
url: /net/convert-onenote-to-pdf/basic-samples/
---

PDF documents are widely used as a standard format of exchanging documents between organizations, government sectors and individuals. It's a popular format so developers are often asked to convert Microsoft OneNote documents to PDF documents. For this purpose, Aspose.Note for .NET supports converting OneNote to PDF documents without using any other component.

## **Save OneNote to PDF using default options**

The following code example demonstrates how to convert OneNote to PDF using the default options.
With default options all pages of the document are saved and present images are compressed by auto selected algorithm.

{{< highlight csharp >}}
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
// Save OneNote to PDF
oneFile.Save(dataDir, SaveFormat.Pdf);
{{< /highlight >}}


### **Save specified page's range of OneNote to PDF**

The following code example demonstrates how to convert a specified range of pages from OneNote to PDF. This range is specified by setting PageIndex and PageCount properties.

The code below saves the first page of OneNote document into a file in PDF format.
             
{{< highlight csharp >}}
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions();

// Set page index: 0 means to start saving from first page.
opts.PageIndex = 0;

// Set page count: 1 means to save only one page.
opts.PageCount = 1;

dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";

// Save OneNote to PDF
oneFile.Save(dataDir, opts);
{{< /highlight >}}

### **Save OneNote to PDF using Jpeg compession for images**

The following code example demonstrates how to convert OneNote to PDF with compressing of all images using JPEG. 
             
{{< highlight csharp >}}
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions
                      {
                         // Use Jpeg compression
                         ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,
                                         
                         // Quality for JPEG compression
                         JpegQuality = 90
                      };

dataDir = dataDir + "sample.pdf";

// Save OneNote to PDF
oneFile.Save(dataDir, opts);
{{< /highlight >}}