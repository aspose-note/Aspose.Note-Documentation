---
title: Convert OneNote documents to PDF and other formats
type: docs
weight: 30
url: /java/convert-onenote-documents-to-pdf-and-other-formats/
---

## **Converting OneNote Document to PDF**
{{% alert color="primary" %}} 

Please note that you cannot set values against the **Application** and **Producer** fields, because of Aspose Ltd. and Aspose.Note for Java x.x will be displayed against these fields.

{{% /alert %}} 

PDF documents are widely used as a standard format of exchanging documents between organizations, government sectors and individuals. It's a popular format so developers are often asked to convert Microsoft OneNote documents to PDF documents. For this purpose, Aspose.Note for Java supports converting OneNote to PDF documents without using any other component. This topic illustrates how this conversion can be done.

Aspose.Note for Java offers the [Document](https://apireference.aspose.com/note/java/com.aspose.note/Document) class that represents a OneNote file. The Document class exposes the Save method that can be called to convert a OneNote document into a PDF document. The [PdfSaveOptions](https://apireference.aspose.com/note/java/com.aspose.note/PdfSaveOptions) class provides options for creating the PDF such as PageIndex, PageCount and others.

This article shows how to:

- [Save all pages as PDF file with the default settings](/note/java/convert-onenote-documents-to-pdf-and-other-formats/).
- [Save the range of pages as PDF](/note/java/convert-onenote-documents-to-pdf-and-other-formats/).
### **Converting OneNote to PDF using the Default Options**
The following example shows how to convert a OneNote into a PDF document using the default options. The default options create a PDF document of the maximum quality.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-load-LoadDocIntoAsposeNoteUsingPdfsaveoptions-LoadDocIntoAsposeNoteUsingPdfSaveOptions.java" >}}

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-load-LoadDocIntoAsposeNoteUsingSaveformat-LoadDocIntoAsposeNoteUsingSaveFormat.java" >}}


### **Converting a Specified Page Range of OneNote to PDF**
The following example shows how to convert a OneNote into a PDF document with a specified page range as provided by the PdfSaveOptions class. It sets the PageIndex and PageCount properties.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-load-ConvertSpecificPageRangeToPdf-SaveRangeOfPagesAsPDF.java" >}}
## **Converting OneNote to Image**
Aspose.Note supports converting OneNote file to images. To use this feature, import the Aspose.Note.Saving namespace into your application project. It has numerous valuable classes for rendering, for example ImageSaveOptions, PdfSaveOptions, and SaveOptions.

Aspose.Note API offers the [Document](https://apireference.aspose.com/note/java/com.aspose.note/Document) class that represents a OneNote file. The Document class exposes the Save method that can be called to convert the OneNote file into an image format. The [ImageSaveOptions](https://apireference.aspose.com/note/java/com.aspose.note/ImageSaveOptions) class provides options for creating PNG, GIF, JPEG or BMP files, such as PageIndex, SaveFormat and others.

This article shows how to:

- [Save OneNote as an image with the default settings](/note/java/convert-onenote-documents-to-pdf-and-other-formats/).
- [Save a particular page of OneNote as an image](/note/java/convert-onenote-documents-to-pdf-and-other-formats/).
- [Set Output Image Resolution](/note/java/convert-onenote-documents-to-pdf-and-other-formats/)
### **Converting OneNote to Image using the Default Options**
The following example shows how to convert a OneNote into an image using the default options.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-load-ConvertToImageUsingDefaultOptions-SaveToImageDefaultOptions.java" >}}
### **Converting a Specific Page in a OneNote Document to Image**
The following example shows how to convert a specific page in a OneNote file into an image using the ImageSaveOptions class. It sets the PageIndex properties.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-load-ConvertSpecificPageToPngImage-ConvertSpecificPageToPng.java" >}}


### **Set Output Image Resolution**
The setResolution method of ImageSaveOptions allows specifying the output image resolution of the converted document.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-load-SetOutputImageResolution-SetOutputImageResolution.java" >}}
