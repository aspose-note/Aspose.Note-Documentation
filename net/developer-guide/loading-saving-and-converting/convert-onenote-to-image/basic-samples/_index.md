---
title: Convert OneNote to image
type: docs
weight: 20
url: /net/convert-onenote-to-image/basic-samples/
---

## **Save OneNote to image in Bmp format using the default options**
The following code example demonstrates how to convert OneNote to image in Bmp format using the default options.
By default only the first page is saved. The saved image has resolution of 96 dpi.

{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Loading-and-Saving-SaveToBmpImageUsingImageSaveOptions.cs" >}}


## **Save OneNote to image in Gif format using the default options**
The following code example demonstrates how to convert OneNote to image in Gif format using the default options.
By default only the first page is saved. The saved image has resolution of 96 dpi.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-SaveToImageDefaultOptions-SaveToImageDefaultOptions.cs" >}}


## **Save a specific page of OneNote to image**
The following code example demonstrates how to convert a specific page of OneNote to image in Png format. The page is specified by setting PageIndex property of [ImageSaveOptions](https://reference.aspose.com/note/net/aspose.note.saving/imagesaveoptions) instance.
The saved image has resolution of 96 dpi.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-ConvertSpecificPageToImage-ConvertSpecificPageToImage.cs" >}}


## **Specify resolution for output image**
The following code example demonstrates how to specify resolution of output image.
The resolution is specified by setting Resolution property of [ImageSaveOptions](https://reference.aspose.com/note/net/aspose.note.saving/imagesaveoptions) instance.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-ConvertSpecificPageToImage-SetOutputImageResolution.cs" >}}


## **Specify quality for output image**
The following code example demonstrates how to convert OneNote to image in Jpeg format with specified compression quality. 
The compression quality is specified by setting Quality property of [ImageSaveOptions](https://reference.aspose.com/note/net/aspose.note.saving/imagesaveoptions) instance. This setting is used when image saved in lossy format.
The image quality can be set from 0 to 100. Zero indicates the lowest quality and 100 gives the highest quality for the image. The default quality value is 90.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-ConvertSpecificPageToImage-SetOutputImageQuality.cs" >}}
