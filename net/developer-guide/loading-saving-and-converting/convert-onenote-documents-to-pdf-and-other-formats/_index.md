---
title: Convert OneNote Documents to PDF and Other Formats
type: docs
weight: 30
url: /net/convert-onenote-documents-to-pdf-and-other-formats/
---

## **Converting OneNote Document to PDF**
{{% alert color="primary" %}} 

Please note that you cannot set values against the **Application** and **Producer** fields, because of Aspose Ltd. and Aspose.Note for .NET x.x will be displayed against these fields.

{{% /alert %}} 

PDF documents are widely used as a standard format of exchanging documents between organizations, government sectors, and individuals. It's a popular format so developers are often asked to convert Microsoft OneNote documents to PDF documents. For this purpose, Aspose.Note for .NET supports converting OneNote to PDF documents without using any other component. This topic illustrates how this conversion can be done.

Aspose.Note for .NET offers the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104359) class that represents a OneNote file. The Document class exposes the Save method that can be called to convert a OneNote document into a PDF document. The [PdfSaveOptions](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Saving.PdfSaveOptions+Class&linkCreation=true&fromPageId=19104359) class provides options for creating the PDF such as PageIndex, PageCount and others.
### **Converting OneNote to PDF using the Default Options**
The following code example demonstrates how to convert a OneNote into a PDF document using the default options. The default options create a PDF document of the maximum quality.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-SaveWithDefaultSettings-SaveWithDefaultSettings.cs" >}}
### **Converting a Specified Page Range of OneNote to PDF**
The following code example demonstrates how to convert a OneNote into a PDF document with a specified page range as provided by the PdfSaveOptions class. It sets the PageIndex and PageCount properties.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-SaveRangeOfPagesAsPDF-SaveRangeOfPagesAsPDF.cs" >}}
## **Converting a OneNote Document to Image**
Aspose.Note supports converting OneNote file to images. To use this feature, import the Aspose.Note.Saving namespace into your application project. It has numerous valuable classes for rendering, for example ImageSaveOptions, PdfSaveOptions and SaveOptions.

Aspose.Note for .NET offers the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104359) class that represents a OneNote file. The Document class exposes the Save method that can be called to convert the OneNote file into an image format. The [ImageSaveOptions](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Saving.ImageSaveOptions+Class&linkCreation=true&fromPageId=19104359) class provides options for creating PNG, GIF, JPEG or BMP files, such as PageIndex, SaveFormat and others.
### **Converting OneNote to Image using the Default Options**
The following code example demonstrates how to convert a OneNote into an image using the default options.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-SaveToImageDefaultOptions-SaveToImageDefaultOptions.cs" >}}
### **Converting a Specific Page in a OneNote to Image**
The following code example demonstrates how to convert a specific page in a OneNote file into an image using the ImageSaveOptions class. It sets the PageIndex properties.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-ConvertSpecificPageToImage-ConvertSpecificPageToImage.cs" >}}
### **Set Output Image Resolution**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-ConvertSpecificPageToImage-SetOutputImageResolution.cs" >}}
### **Set Output Image Quality**
The image quality can be set from 0 to 100. Zero indicates the lowest quality and 100 gives the highest quality for the image. The default quality value is 90.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-ConvertSpecificPageToImage-SetOutputImageQuality.cs" >}}
