---
title: Converting OneNote to PDF using the Default Options
type: docs
weight: 30
url: /net/convert-onenote-documents-to-pdf-format/using-default-options/
---

The following code example demonstrates how to convert a OneNote into a PDF document using the default options.
With default options all pages of the document are saved and present images are compressed by auto selected algorithm.

{{< highlight csharp >}}
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
// Save the document as PDF
oneFile.Save(dataDir, SaveFormat.Pdf);
{{< /highlight >}}