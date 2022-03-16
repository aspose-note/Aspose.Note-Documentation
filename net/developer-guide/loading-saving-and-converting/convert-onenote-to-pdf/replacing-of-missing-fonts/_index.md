---
title: Convert OneNote to PDF with replacing of missing fonts
type: docs
weight: 30
url: /net/convert-onenote-to-pdf/replacing-of-missing-fonts/
description: Convert OneNote to PDF using C# API and learn to set default font or replace missing fonts or set fonts from stream. 
---

PDF documents are widely used as a standard format of exchanging documents between organizations, government sectors and individuals. It's a popular format so developers are often asked to convert Microsoft OneNote documents to PDF documents. For this purpose, Aspose.Note for .NET supports converting OneNote to PDF documents without using any other component.
This topic shows how to save a Document using a font that is not available under the current machine.

If a OneNote document uses a font that is not available under the current machine then you can specify to substitute it by another widely used font.

## **How to set default font name**

The sample below shows how to convert OneNote to PDF while substitututing missing fonts by Times New Roman font that is available on most machines.

{{< highlight csharp >}}
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
            
// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Convert OneNote to PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
{{< /highlight >}}


## **How to set a font from a file as default**

The sample below shows how to convert OneNote to PDF while substitututing missing fonts by a font located in a specified file.

{{< highlight csharp >}}
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Convert OneNote to PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
{{< /highlight >}}


## **How to set a font from a stream as default**

The sample below shows how to convert OneNote to PDF while substitututing missing fonts by a font from provided stream.

{{< highlight csharp >}}
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Convert OneNote to PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
{{< /highlight >}}

