---
title: Introduction
type: docs
weight: 10
url: /java/introduction/
description: Hello World example to create OneNote document from scratch using Java library or API.  You can add OneNote page, outline, outline element and text dynamically using Java.
---

## **Create a Hello World OneNote Document using the API**
This article explains how to create a OneNote document from scratch using the simple APIs provided by Aspose.Note for Java. To create a OneNote document, add page, outline, outline element and text dynamically using the set of classes packaged in the [Aspose.Note](https://reference.aspose.com/note/java) namespace.

Please follow these steps to create a OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](https://reference.aspose.com/note/java/com.aspose.note/Document) class that represents a OneNote document.
1. If you have purchased a license, then embed the code to apply for that license with the help of the **License** class.
1. Initialize one object of [Page](https://reference.aspose.com/note/java/com.aspose.note/Page), [Outline](https://reference.aspose.com/note/java/com.aspose.note/Outline), [OutlineElement](https://reference.aspose.com/note/java/com.aspose.note/OutlineElement) and [RichText](https://reference.aspose.com/note/java/com.aspose.note/RichText) classes bypassing the [Document](https://reference.aspose.com/note/java/com.aspose.note/Document) class object. 
   Calling the AppendChildLast method of the [OutlineElement](https://reference.aspose.com/note/java/com.aspose.note/OutlineElement), [Outline](https://reference.aspose.com/note/java/com.aspose.note/Outline), [Page](https://reference.aspose.com/note/java/com.aspose.note/Page) and [Document](https://reference.aspose.com/note/java/com.aspose.note/Document) classes adds an appropriate new node that can be further used to add new nodes to the OneNote document.
1. The [TextStyle](https://reference.aspose.com/note/java/com.aspose.note/TextStyle) class defines the text formatting. Similarly, the DefaultStyle property exposed by [RichText](https://reference.aspose.com/note/java/com.aspose.note/RichText) class allows applying to format on the text.
1. Generate the OneNote document by calling the Save method of the [Document](https://reference.aspose.com/note/java/com.aspose.note/Document) object.

These articles show how to:

- [Create a OneNote Document with Simple RichText](/note/java/introduction/#create-a-onenote-document-with-simple-richtext).
- [Create a OneNote Document with Formatted RichText](/note/java/introduction/#create-a-onenote-document-with-formatted-richtext).
### **Create a OneNote Document with Simple RichText**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-introduction-CreateOneNoteDocumentWithSimpleRichText-CreateDocWithSimpleRichText.java" >}}
### **Create a OneNote Document with Formatted RichText**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-introduction-CreateOneNoteDocumentWithFormattedRichText-CreateDocWithFormattedRichText.java" >}}



