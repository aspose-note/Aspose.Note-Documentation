---
title: Create or Work with OneNote NoteBook in C# API
linktitle: Working with OneNote NoteBook
type: docs
weight: 50
url: /net/working-with-onenote-notebook/
keywords: create onenote notebook c#
description: OneNote NoteBook C# API lets you create or save NoteBook to Stream, load NoteBook from file, export NoteBook to Image with Options and export NoteBook to PDF
---

## **Creating and Saving a Notebook**
The Notebook class exposed by the API lets you create a notebook from scratch and save it as OneNote Notebook (.onetoc2). OneNote notebook can be created using the default constructor of Notebook class. This article shows creating and saving a Notebook document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-CreateNoteBook-CreateNoteBook.cs" >}}
### **Saving Notebook to Stream**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-SaveNotebookToStream-SaveNotebookToStream.cs" >}}
### **Support of Password Protected Documents Writing as Part of .onetoc2 Notebook**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-WritingPasswordProtectedDoc-WritingPasswordProtectedDoc.cs" >}}
## **Reading Notebook File**
The .onetoc2 file format represents the saved table of contents for the OneNote document. The Notebook class can be used to read this type of Microsoft .one file format and parse it further. The following code sample shows the usage of this class for use.
### **Loading Notebook File**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-LoadOneNoteDoc-LoadOneNoteDoc.cs" >}}
### **Loading Notebook from Stream**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-LoadFromStream-LoadFromStream.cs" >}}
### **Loading Notebook File with LoadOptions**
By default, notebook's child documents are loaded "lazily", i.e. their loading is postponed until direct access to a specific child. An alternative approach is to load all children at once. The last can be achieved by passing to the Notebook constructor NotebookLoadOptions with InstantLoading flag set to true. Following code snippets demonstrate both approaches.
#### **Loading Notebook with Lazy Loading Option**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-LoadingNotebookFilewithLoadOptions-LoadingNotebookFilewithLoadOptions.cs" >}}
#### **Loading Notebook Instantly**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-LoadingNotebookInstantly-LoadingNotebookInstantly.cs" >}}
#### **Loading Password Protected Documents as a part of .onetoc2 Notebook**
A Notebook having password protected .One documents can be loaded with the help of LoadOptions class of the API specifying the password.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-LoadingPasswordProtectedDoc-LoadingPasswordProtectedDoc.cs" >}}
## **Adding a Child Node to OneNote Notebook**
Aspose.Note API lets you add/append a child node at first or last to a OneNote Notebook. The AppendChildLast or AppendChildFirst methods exposed by the Notebook class allows you to achieve this.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-AddChildNode-AddChildNode.cs" >}}
## **Remove a Child Node From OneNote Notebook**
Aspose.Note API provides the capability to remove a child node from OneNote notebook. The RemoveChild method exposed by the API's Notebook class lets you remove a child node that is meant to be removed from the Notebook.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-RemoveChildNode-RemoveChildNode.cs" >}}
## **Converting Notebook Document to Image**
Aspose.Note API provides the capability to convert Notebook documents (.onetoc2) to image. The API can export the document to image directly or we can also specify additional save options using the NotebookImageSaveOptions class.
### **Exporting Notebook to Image**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-ConvertToImage-ConvertToImage.cs" >}}
### **Exporting Notebook to Image with Options**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-ConvertToImageWithOptions-ConvertToImageWithOptions.cs" >}}
### **Export to Image as a Flattened Notebook**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-ConvertToImageAsFlattenedNotebook-ConvertToImageAsFlattenedNotebook.cs" >}}
## **Converting Notebook Document to PDF**
Aspose.Note API provides the capability to convert Notebook documents (.onetoc2) to PDF format. The API can export the document to PDF directly or we can also specify additional save options using the NotebookPdfSaveOptions class. This article shows all the approaches to export Notebook to PDF.

{{% alert color="primary" %}} 

Please note that you cannot set values against the **Application** and **Producer** fields, because of Aspose Ltd. and Aspose.Note for .NET x.x will be displayed against these fields.

{{% /alert %}} 
### **Exporting Notebook to PDF**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-ConvertToPDF-ConvertToPDF.cs" >}}
### **Exporting Notebook to PDF with Options**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-ConvertToPDFWithOptions-ConvertToPDFWithOptions.cs" >}}
### **Export to PDF as a Flattened Notebook**
Aspose.Note API can be used to export a OneNote notebook as a Flattened PDF which exports all children to a single directory.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-ConvertToPDFAsFlattened-ConvertToPDFAsFlattened.cs" >}}
## **Retrieve Documents from OneNote Notebook**
The following code snippet demonstrates how to get all documents which are presented in the entire MS OneNote notebook including child notebooks.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-RetrieveDocumentsfromOneNoteNotebook-RetrieveDocumentsfromOneNoteNotebook.cs" >}}
## **Read RichText Nodes from Microsoft OneNote Notebook**
The following code snippet demonstrates how to print all RichText nodes from MS OneNote notebook:

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-NoteBook-ReadRichText-ReadRichText.cs" >}}
