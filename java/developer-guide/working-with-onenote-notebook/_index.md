---
title: Working with OneNote Notebook
type: docs
weight: 40
url: /java/working-with-onenote-notebook/
---

## **Creating and Saving A Notebook**
The Notebook class exposed by the API lets you create a notebook from scratch and save it as OneNote Notebook (.onetoc2). OneNote notebook can be created using the default constructor of Notebook class. This article shows creating and saving a Notebook document.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-CreatandSaveANotebook-CreatandSaveANotebook.java" >}}
### **Saving Notebook to Stream**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-SaveNotebooktoStream-SaveNotebooktoStream.java" >}}
### **Support of Password Protected Documents Writing as Part of .onetoc2 Notebook**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-WritingPasswordProtectedDoc-WritingPasswordProtectedDoc.java" >}}
## **Reading Notebook File**
The Notebook class exposed by the API lets you read a OneNote Notebook (.onetoc2) file from disc. The NotebookLoadOptions class provides further options to load the file with user-specified options.
### **Loading Notebook File**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-LoadingNotebook-LoadingNotebook.java" >}}
### **Loading Notebook File from Stream**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-LoadFilefromStream-LoadFilefromStream.java" >}}
### **Loading Notebook File with LoadOptions**
By default, notebook's child documents are loaded "lazily", i.e. their loading is postponed until direct access to a specific child. An alternative approach is to load all children at once. The last can be achieved by passing to the Notebook constructor NotebookLoadOptions with the InstantLoading flag set to true. The following code snippets demonstrate both approaches.
#### **Loading Notebook with Lazy Loading Option**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-LoadingNotebookFilewithLoadOptions-LoadingNotebookFilewithLoadOptions.java" >}}
#### **Loading Notebook Instantly**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-LoadingNotebookInstantly-LoadingNotebookInstantly.java" >}}

{{% alert color="primary" %}} 

In the current implementation, lazy loading implemented only for OneNote 2010 child documents/notebooks. OneNote Online first-level child documents/notebooks are always loaded instantly.

For instance, if there is a hierarchy structure:

- Root Notebook (2010)

— Section 1 Level 1 (2010)

— Section 2 Level 1 (Online)

— Notebook 1 Level 1 (2010)

----- Section 1 Level 2 (Online)

— Notebook 2 Level 1 (Online)

----- Section 1 Level 2 (Online)

----- Section 2 Level 2 (2010)

Then the only children will be loaded instantly are: Root Notebook -> Section 2 Level 1, Root Notebook -> Notebook 2 Level 1 and Root Notebook -> Notebook 2 Level 1 -> Section 1 Level 2.

Note that "Root Notebook -> Notebook 1 Level 1 -> Section 1 Level 2" is not loaded at the same time as "Root Notebook"; instead it will be loaded instantly while "Root Notebook -> Notebook 1 Level 1" is loading, as it is the first-level child for the mentioned notebook and the last is not Online itself.

{{% /alert %}} 
#### **Loading Password Protected Documents as a part of .onetoc2 Notebook**
A password-protected notebook can be loaded with the help of LoadOptions class of the API specifying the password.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-LoadPasswordProtectedDocuments-LoadingPasswordProtectedDoc.java" >}}
## **Adding a Child Node to OneNote Notebook**
Aspose.Note API lets you add/append a child node to a OneNote Notebook. The appendChildLast method exposed by the Notebook class allows you to achieve this.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-AddChildNode-AddChildNode.java" >}}
## **Remove a Child Node From OneNote Notebook**
Aspose.Note API provides the capability to remove a child node from OneNote notebook. The removeChild method exposed by the API's Notebook class lets you remove a child node that is meant to be removed from the Notebook.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-RemoveChildNode-RemoveChildNode.java" >}}
## **Converting Notebook Document to Image**
Aspose.Note API provides the capability to convert Notebook documents (.onetoc2) to image. The API can export the document to image directly or we can also specify additional save options using the NotebookImageSaveOptions class. This article shows all the approaches to export Notebook to the image.
### **Exporting Notebook to Image**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-ConvertToImage-ConvertToImage.java" >}}
### **Exporting Notebook to Image with Options**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-ConvertToImageWithOptions-ConvertToImageWithOptions.java" >}}
### **Export to Image as a Flattened Notebook**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-ConvertToImageAsFlattenedNotebook-ConvertToImageAsFlattenedNotebook.java" >}}
## **Converting Notebook Document to PDF**
Aspose.Note API provides the capability to convert Notebook documents (.onetoc2) to PDF format. The API can export the document to PDF directly or we can also specify additional save options using the NotebookPdfSaveOptions class. This article shows all the approaches to export Notebook to PDF.

Please note that you cannot set values against the **Application** and **Producer** fields, because of Aspose Ltd. and Aspose.Note for Java x.x will be displayed against these fields.


### **Exporting Notebook to PDF**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-ConvertToPDF-ConvertToPDF.java" >}}
### **Exporting Notebook to PDF with Options**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-ConvertToPDFWithOptions-ConvertToPDFWithOptions.java" >}}
### **Export to PDF as a Flattened Notebook**
Aspose.Note API can be used to export a OneNote notebook as a Flattened PDF which exports all children to a single directory.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-ExportNotebookToPDFAsFlattened-ExportNotebookToPDFAsFlattened.java" >}}
## **Retrieve Documents from OneNote Notebook**
The following code snippet demonstrates how to get all documents which are presented in the entire MS OneNote notebook including child notebooks.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-RetrieveDocumentsfromOneNoteNotebook-RetrieveDocumentsfromOneNoteNotebook.java" >}}
## **Read RichText Nodes from Microsoft OneNote Notebook**
The following code snippet demonstrates how to print all RichText nodes from MS OneNote notebook:

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-Notebook-ReadRichText-ReadRichText.java" >}}
