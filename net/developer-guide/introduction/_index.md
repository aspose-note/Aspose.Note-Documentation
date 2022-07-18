---
title: Introduction
type: docs
weight: 10
url: /net/introduction/
---

## **Create a Hello World OneNote document Using API**
This article explains how to create a OneNote document from scratch using the simple APIs provided by Aspose.Note for .NET. To create a OneNote document, add page, outline, outline element and text dynamically using the set of classes packaged in the [Aspose.Note](https://reference.aspose.com/note/net/aspose.note) namespace.

Please follow these steps to create a OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](https://reference.aspose.com/note/net/aspose.note/document) class that represents a OneNote document.
1. If you have purchased a license, then embed the code to apply for that license with the help of the [License](https://reference.aspose.com/note/net/aspose.note/license) class.
1. Initialize one object of [Page](https://reference.aspose.com/note/net/aspose.note/page), [Outline](https://reference.aspose.com/note/net/aspose.note/outline), [OutlineElement](https://reference.aspose.com/note/net/aspose.note/outlineelement) and [RichText](https://reference.aspose.com/note/net/aspose.note/richtext) classes bypassing the [Document](https://reference.aspose.com/note/net/aspose.note/document) class object. 
   Calling the AppendChild method of the [OutlineElement](https://reference.aspose.com/note/net/aspose.note/outlineelement), [Outline](https://reference.aspose.com/note/net/aspose.note/outline), [Page](https://reference.aspose.com/note/net/aspose.note/page) and [Document](https://reference.aspose.com/note/net/aspose.note/document) classes adds an appropriate new node that can be further used to add new nodes to the OneNote document.
1. The [ParagraphStyle](https://reference.aspose.com/note/net/aspose.note/paragraphstyle) class defines the text formatting. Similarly, the ParagraphStyle property exposed by [RichText](https://reference.aspose.com/note/net/aspose.note/richtext) class allows applying to format on the text. Text style settings to be used if there is no matching TextStyle object in Styles collection either this object doesn't specify a needed setting.
1. Generate the OneNote document by calling the Save method of the [Document](https://reference.aspose.com/note/net/aspose.note/document) object.
### **Create a OneNote Document with Simple RichText**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-CreateDocWithSimpleRichText-CreateDocWithSimpleRichText.cs" >}}
### **Create a OneNote Document with Formatted RichText**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-CreateDocWithFormattedRichText-CreateDocWithFormattedRichText.cs" >}}
