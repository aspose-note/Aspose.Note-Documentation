---
title: Convert OneNote to image in various color modes
type: docs
weight: 20
url: /net/convert-onenote-to-image/convert-to-colormode/
---

## **Save OneNote to a grayscale image in Png format**
The following code example demonstrates how to convert a OneNotet to a grayscale image. 
The ColorMode property of [ImageSaveOptions](https://reference.aspose.com/note/net/aspose.note.saving/imagesaveoptions) instance is used to indicate that output image should be grayscale.

{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Loading-and-Saving-SaveToGrayscaleImage.cs" >}}


## **Save OneNote to a binary image**
There are various methods for image's binarization. Aspose.Note supports two well-known methods: thresholding and Otsu's method.


The following code example demonstrates how to convert a OneNote to a binary image using thresholding method.
The BinarizationOptions property of [ImageSaveOptions](https://reference.aspose.com/note/net/aspose.note.saving/imagesaveoptions) instance is used to indicate that thresholding method should be applied.

{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Loading-and-Saving-SaveToBinaryImageUsingFixedThreshold.cs" >}}


The following code example demonstrates how to convert a OneNote to a binary image using Otsu's method.
The BinarizationOptions property of [ImageSaveOptions](https://reference.aspose.com/note/net/aspose.note.saving/imagesaveoptions) instance is used to indicate that Otsu's method should be applied.

{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Loading-and-Saving-SaveToBinaryImageUsingOtsuMethod.cs" >}}


## **Save OneNote to a binary image in TIFF format with specified compression and default binarization options**
The following code example demonstrates how to convert a OneNote to a binary image and save it in TIFF format using Jpeg compression. 
The ColorMode property of [ImageSaveOptions](https://reference.aspose.com/note/net/aspose.note.saving/imagesaveoptions) instance is used to indicate that output image should be binary.
The TiffCompression property of [ImageSaveOptions](https://reference.aspose.com/note/net/aspose.note.saving/imagesaveoptions) instance is used to indicate that Jpeg compression should be applied.
By default thresholding binarization method with threshold 128 is applied.

{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Loading-and-Saving-SaveToTiffImageUsingImageSaveOptions.cs-SaveToTiffUsingJpegCompression" >}}


The following code example demonstrates how to convert a OneNote to a binary image and save it in TIFF format using CCITT Group 3 fax compression. 
The TiffCompression property of [ImageSaveOptions](https://reference.aspose.com/note/net/aspose.note.saving/imagesaveoptions) instance is used to indicate that CCITT Group 3 fax compression should be applied.

{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Loading-and-Saving-SaveToTiffImageUsingImageSaveOptions.cs-SaveToTiffUsingCcitt3Compression" >}}
