---
title: Working with Images
type: docs
weight: 60
url: /java/working-with-images/
---

## **Extract Images from a OneNote Document**
{{% alert color="primary" %}} 

All images are stored inside image nodes in a OneNote document.

{{% /alert %}} 
### **Extract Images**
To extract all images or from a OneNote document, follow these steps:

1. Use the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document).getChildNodes method to select all Image nodes.
1. Iterate through the resulting Image node collections.
1. Extract image bytes array using the Image.Bytes property.
1. Save image bytes to a file.

This example shows how to extract images from a OneNote document and save them as files.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-images-ExtractImages-ExtractImages.java" >}}
## **Get Information of Each Image from the OneNote Document**
The [Image](http://www.aspose.com/api/java/note/com.aspose.note/classes/Image) class provides all the image properties for images in OneNote documents. All the images of the OneNote file are contained by image nodes in the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) object.
### **Get Information**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-images-GetImageInfo-GetInformationOfImages.java" >}}
## **Adding Image to a OneNote Document Page and Saving as PDF**
Aspose.Diagram for JAVA APIs now allows inserting an image anywhere on the OneNote document.

These examples show how to:

- [Insert an Image in an Existing OneNote Document](/note/java/working-with-images/).
- [Build a OneNote Document from Scratch and Insert an Image](/note/java/working-with-images/).
- [Build a OneNote Document from Scratch and Insert an Image using an image stream](/note/java/working-with-images/).
- [Support for Alternative Text in Image](/note/java/working-with-images/)
### **Insert an Image in an Existing OneNote Document**
To insert an image on a OneNote document, follow these steps:

1. Use the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/document/methods/getFirstChild\(\)/).getFirstChild() property to get the first page.
1. Use the [Image](http://www.aspose.com/api/java/note/com.aspose.note/classes/Image) class constructor to load the image.
1. Use the [Image](http://www.aspose.com/api/java/note/com.aspose.note/classes/Image).getWidth() and [Image](http://www.aspose.com/api/java/note/com.aspose.note/classes/Image).getHeight() properties to adjust size of the image.
1. Use the [Image](http://www.aspose.com/api/java/note/com.aspose.note/classes/Image).getVerticalOffset() and [Image](http://www.aspose.com/api/java/note/com.aspose.note/classes/Image).getHorizontalOffset() properties to set location of the image.
1. Use the [Page](http://www.aspose.com/api/java/note/com.aspose.note/classes/Page).appendChild() property to insert the image.
1. Save a OneNote document.

This example shows how to insert an image on a OneNote document and save them as files.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-images-InsertanImage-InsertImage.java" >}}


### **Build a OneNote Document from the Scratch and Insert an Image**
This example shows how to build a new OneNote document and insert an image by file path.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-images-BuildDocAndInsertImage-BuildDocAndInsertImage.java" >}}
### **Build a OneNote Document from the Scratch and Insert an Image using an Image Stream**
This example shows how to build a new OneNote document and insert an image using the image stream.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-images-BuildDocAndInsertImageUsingImageStream-BuildDocAndInsertImageUsingImageStream.java" >}}
### **Support for Image Alternative Text**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-images-AlternativeText-ImageAlternativeText.java" >}}
### **Link an Image to Hyperlink**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-images-AddHyperlinkToImage-AddHyperlinkToImage.java" >}}
