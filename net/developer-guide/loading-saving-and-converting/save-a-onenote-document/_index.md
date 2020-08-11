---
title: Save a OneNote Document
type: docs
weight: 20
url: /net/save-a-onenote-document/
---

## **Saving a Document to OneNote Format**
**How does it work?**

The save method exposed by the API lets you save the document to OneNote format. The following three overloaded members provide the option to save the document in OneNote format.

- Save(string)
- Save(string, OneSaveOptions)
- Save(string, SaveFormat)

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-SaveDocToOneNoteFormat-SaveDocToOneNoteFormat.cs" >}}
### **Saving a Document Using Save Options**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-SaveDocToOneNoteFormatUsingOnesaveoptions-SaveDocToOneNoteFormatUsingOnesaveoptions.cs" >}}
### **Saving a Document Using Save Format**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-SaveDocToOneNoteFormatUsingSaveFormat-SaveDocToOneNoteFormatUsingSaveFormat.cs" >}}
## **Save OneNote Document to a Stream**
Users can pass a stream object to the Document.Save(Stream, SaveFormat) method. When saving to a stream, you must specify the save format explicitly.

The following code example demonstrates how to save a document to a stream.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-SaveToStream-SaveToStream.cs" >}}
## **Specify OneNote Save Options**
There are overloaded Document.Save methods that accept a SaveOptions object. This should be an object of a class derived from the SaveOptions class. Each save format has a corresponding class that holds save options for that format, for example, there is PdfSaveOptions for SaveFormat.Pdf and OneSaveOptions for SaveFormat.One.

The following code example demonstrates how to set save options before saving a document to PDF.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-SpecifySaveOptions-SpecifySaveOptions.cs" >}}
