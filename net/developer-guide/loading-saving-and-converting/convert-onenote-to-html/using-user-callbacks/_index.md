---
title: Convert OneNote to Html using user saving callbacks
type: docs
weight: 20
url: /net/convert-onenote-to-html/using-user-callbacks/
---

Time to time it is useful to have full control over storing all Html generated content.
For this reason Aspose.Note have an option to provide user-defined callbacks for saving of pages([PageSavingArgs](https://apireference.aspose.com/note/net/aspose.note.saving.html/pagesavingargs)), style sheets([CssSavingArgs](https://apireference.aspose.com/note/net/aspose.note.saving.html/csssavingargs)), images([ImageSavingArgs](https://apireference.aspose.com/note/net/aspose.note.saving.html/imagesavingargs)) and fonts([FontSavingArgs](https://apireference.aspose.com/note/net/aspose.note.saving.html/fontsavingargs)).

## **Save OneNote to Html using user saving callbacks**

The following code example demonstrates how to convert OneNote to Html with storing all resources(css/fonts/images) by using user-defined callbacks.

The code below creates 'documentFolder' folder containing document.html, 'css' folder with 'style.css' file, 'images' folder with images and 'fonts' folder with fonts.
'style.css' file will contain at the end the following string "/* This line is appended to stream manually by user */"

{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Loading-and-Saving-CreateOneNoteDocAndSaveToHTML.cs-SaveAsHTMLToMemoryStreamWithCallBacksToSaveResources" >}}
