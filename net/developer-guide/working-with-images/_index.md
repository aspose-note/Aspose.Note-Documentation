---
title: Working with Images
type: docs
weight: 70
url: /net/working-with-images/
---

## **Extract Images from a OneNote Document**
All images are stored inside image nodes in a OneNote document.
### **Extract Images**
To extract all images or from a OneNote document, follow these steps:

1. Use the [Document](http://www.aspose.com/api//net/note/aspose.note/document).GetChildNodes method to select all Image nodes.
1. Iterate through the resulting Image node collections.
1. Extract image bytes array using the Image.Bytes property.
1. Save image bytes to a file.

The code example given below demonstrates how to extract images from a OneNote document and save them as files.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Images-ExtractImages-ExtractImages.cs" >}}
## **Get Information of Each Image from the OneNote Document**
The [Image](http://www.aspose.com/api//net/note/aspose.note/image) class provides all the image properties for images in OneNote documents. All the images of the OneNote file are contained by image nodes in the [Document](http://www.aspose.com/api//net/note/aspose.note/document) object.
### **Get Information**
The code example given below demonstrates how to get information about each image from a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Images-GetInformationOfImages-GetInformationOfImages.cs" >}}
## **Insert an Image on a OneNote Document Page**
Aspose.Diagram for .NET APIs now allows inserting an image anywhere on the OneNote document.

An image can be inserted in the following ways.
### **Insert an Image in an Existing OneNote Document**
To insert an image on a OneNote document, follow these steps:

1. Use the [Document](http://www.aspose.com/api//net/note/aspose.note/document).FirstChild property to get the first page.
1. Use the [Image](http://www.aspose.com/api/net/note/aspose.note/image) class constructor to load the image.
1. Use the [Image](http://www.aspose.com/api/net/note/aspose.note/image).Width and [Image](http://www.aspose.com/api/net/note/aspose.note/image).Height properties to adjust the size of the image.
1. Use the [Image](http://www.aspose.com/api/net/note/aspose.note/image).VerticalOffset and [Image](http://www.aspose.com/api/net/note/aspose.note/image).HorizontalOffset properties to set the location of the image.
1. Use the [Page](http://www.aspose.com/api/net/note/aspose.note/page).AppendChild property to insert the image.
1. Save a OneNote document.

The code example given below demonstrates how to insert an image on a OneNote document and save them as files.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Images-InsertImage-InsertImage.cs" >}}
### **Build a OneNote Document from Scratch and Insert an Image**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Images-BuildDocAndInsertImage-BuildDocAndInsertImage.cs" >}}
### **Build a OneNote Document from the Scratch and Insert an Image using an Image Stream**
This code example shows how to build a new OneNote document and insert an image using the image stream.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Images-BuildDocAndInsertImageUsingImageStream-BuildDocAndInsertImageUsingImageStream.cs" >}}
### **Support for Image Alternative Text**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Images-ImageAlternativeText-ImageAlternativeText.cs" >}}
### **Link an Image to Hyperlink**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Images-ImageWithHyperlink-ImageWithHyperlink.cs" >}}
