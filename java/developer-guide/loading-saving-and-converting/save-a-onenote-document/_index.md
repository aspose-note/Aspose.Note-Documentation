---
title: Save a OneNote Document
type: docs
weight: 20
url: /java/save-a-onenote-document/
---

## **Saving a Document to OneNote Format**
**How does it work?**

The save method exposed by the API lets you save the document to OneNote format. The following three overloaded members provide the option to save the document in OneNote format.

- save(string)
- save(string, OneSaveOptions)
- save(string, SaveFormat)

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-load-SaveDocToOneNoteFormat-SaveDocToOneNoteFormat.java" >}}
### **Saving a Document Using Save Options**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-load-SaveDocToOneNoteFormatUsingOnesaveoptions-SaveDocToOneNoteFormatUsingOneSaveOptions.java" >}}
### **Saving a Document Using Save Format**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-load-SaveDocToOneNoteFormatUsingSaveformat-SaveDocToOneNoteFormatUsingSaveFormat.java" >}}
## **Save OneNote Document to a Stream**
Users can pass a stream object to the Document.save(Stream, SaveFormat) method. When saving to a stream, you must specify the save format explicitly.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-load-SaveOneNoteDocToStream-SaveOneNoteDocToStream.java" >}}
## **Specify OneNote Save Options**
There are overloaded Document.save methods that accept a SaveOptions object. This should be an object of a class derived from the SaveOptions class. Each save format has a corresponding class that holds save options for that format. For example, there is PdfSaveOptions for SaveFormat.Pdf and OneSaveOptions for SaveFormat.One.

The code below shows how to set save options before saving a document to PDF.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-load-SpecifySaveOptions-SpecifySaveOptions.java" >}}
## **Working with Locales**
Aspose.Note provides an opportunity to set locales using [setLocale ](https://apireference.aspose.com/java/note/com.aspose.note/LocaleOptions#setLocale-java.util.Locale-)method under [LocaleOptions](https://apireference.aspose.com/java/note/com.aspose.note/LocaleOptions) class.

The code below shows how to set locales options before saving a document.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-locales-WorkingWithLocales-WorkingWithLocales.java" >}}
