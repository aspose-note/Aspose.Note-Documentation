---
title: Introduction
type: docs
weight: 10
url: /java/introduction/
---

## **Create a Hello World OneNote Document using the API**
This article explains how to create a OneNote document from scratch using the simple APIs provided by Aspose.Note for Java. To create a OneNote document, add page, outline, outline element and text dynamically using the set of classes packaged in the [Aspose.Note](http://www.aspose.com/api/java/note/com.aspose.note/index) namespace.

Please follow these steps to create a OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) class that represents a OneNote document.
1. If you have purchased a license, then embed the code to apply for that license with the help of the [License](http://www.aspose.com/api/java/note/com.aspose.note/classes/License) class.
1. Initialize one object of [Page](http://www.aspose.com/api/java/note/com.aspose.note/classes/Page), [Outline](http://www.aspose.com/api/java/note/com.aspose.note/classes/Outline), [OutlineElement](http://www.aspose.com/api/java/note/com.aspose.note/classes/OutlineElement) and [RichText](http://www.aspose.com/api/java/note/com.aspose.note/classes/RichText) classes bypassing the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) class object. 
   Calling the AppendChildLast method of the [OutlineElement](http://www.aspose.com/api/java/note/com.aspose.note/classes/OutlineElement), [Outline](http://www.aspose.com/api/java/note/com.aspose.note/classes/Outline), [Page](http://www.aspose.com/api/java/note/com.aspose.note/classes/Page) and [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) classes adds an appropriate new node that can be further used to add new nodes to the OneNote document.
1. The [TextStyle](http://www.aspose.com/api/java/note/com.aspose.note/classes/TextStyle) class defines the text formatting. Similarly, the DefaultStyle property exposed by [RichText](http://www.aspose.com/api/java/note/com.aspose.note/classes/RichText) class allows applying to format on the text.
1. Generate the OneNote document by calling the Save method of the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) object.

These articles show how to:

- [Create a OneNote Document with Simple RichText](/note/java/introduction-html/).
- [Create a OneNote Document with Formatted RichText](/note/java/introduction-html/).
### **Create a OneNote Document with Simple RichText**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-introduction-CreateOneNoteDocumentWithSimpleRichText-CreateDocWithSimpleRichText.java" >}}
### **Create a OneNote Document with Formatted RichText**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-introduction-CreateOneNoteDocumentWithFormattedRichText-CreateDocWithFormattedRichText.java" >}}



