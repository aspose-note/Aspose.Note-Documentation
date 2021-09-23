---
title: Working with Text
type: docs
weight: 80
url: /net/working-with-text/
---

## **Extract Text from OneNote Document**
One of the tasks that developers need to perform is extracting text from an OneNote document. [Aspose.Note for .NET](https://products.aspose.com/note/net) allows developers to extract text from OneNote document in various ways.

Aspose.Note for .NET offers the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents the OneNote file. The simple LINQ can be used to extract text from the OneNote document.
### **Extracting All Text from OneNote Document**
This example works as follows:

1. Create an object of the Document class.
1. Call the LINQ-based Code to extract text
1. Display text on the output screen.

The following code example demonstrates how to extract all text from the OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-ExtractingAllText-ExtractingAllText.cs" >}}
### **Extracting Text from a Specified Page of OneNote Document**
This example works as follows:

1. Create an object of the Document class.
1. Filter out a list of page nodes.
1. Retrieve the page node by index.
1. Call the LINQ-based Code to extract text
1. Display the text on the output screen.

The following code example demonstrates how to extract text from a specified page in OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-ExtractingTextFromAPage-ExtractingTextFromAPage.cs" >}}
## **Replace Text in Pages of OneNote Document**
Aspose.Note for .NET supports finding and then replacing text within OneNote document. Aspose.Note for .NET offers the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents the OneNote file.
### **Replace Text on All Pages**
The following code example demonstrates how to replace text on all pages.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-ReplaceTextOnAllPages-ReplaceTextOnAllPages.cs" >}}
### **Replace Text on a Particular Page**
The following code example demonstrates how to replace text on a particular page.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-ReplaceTextOnParticularPage-ReplaceTextOnParticularPage.cs" >}}
## **Retrieve Bullet or Number List Properties**
[Aspose.Note for .NET](https://products.aspose.com/note/net) provides comprehensive support for Microsoft OneNote lists. Developers can access a number of list properties, such as font name, numbering format, and many others.
### **Retrieving Properties**
Aspose.Note for .NET offers the [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement) class that represents an outline inside a OneNote document. The OutlineElement class exposes the NumberList property that can be called to extract bullet or numbered list properties. The following example shows how to extract bullet or numbered list properties from a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-RetrieveBulletOrNumberList-RetrieveBulletOrNumberList.cs" >}}
## **Apply Bullets on the Text**
Arranging texts in bullet form is a very common approach. Aspose.Note for .NET APIs allows developers to arrange text items in bullets.

Aspose.Note for .NET offers the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents a OneNote file. Writing text to a OneNote document page involves creating an [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement), which offers NumberList property to define the bullet.

Please see a brief description to add and apply bullets on the text in OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents a OneNote document.
1. Initialize three objects of [Page](https://apireference.aspose.com/note/net/aspose.note/page) class and set their levels.
1. Initialize the objects of [Outline](https://apireference.aspose.com/note/net/aspose.note/outline), [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement) and [RichText](https://apireference.aspose.com/note/net/aspose.note/richtext) classes. 
   Setting the NumberList property of the [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement) class adds bullets.
1. The [ParagraphStyle](https://apireference.aspose.com/note/net/aspose.note/paragraphstyle) class defines the text formatting.
1. Generate the OneNote document by calling the Save method of the [Document](https://apireference.aspose.com/note/net/aspose.note/document) object.

The following code example demonstrates how to apply a bullet on the OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-ApplyBulletsOnText-ApplyBulletsOnText.cs" >}}
## **Apply Numbering on the Text**
Arranging texts in numbering form is a very common approach. Aspose.Note for .NET APIs allows developers to arrange text items in numbering.

Aspose.Note for .NET offers the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents a OneNote file. Writing text to a OneNote document page involves creating an [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement), which offers NumberList property to define the bullet.

Please see a brief description to add and apply bullets on the text in OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents a OneNote document.
1. Initialize three objects of [Page](https://apireference.aspose.com/note/net/aspose.note/page) class and set their levels.
1. Initialize the objects of [Outline](https://apireference.aspose.com/note/net/aspose.note/outline), [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement) and [RichText](https://apireference.aspose.com/note/net/aspose.note/richtext) classes. 
   Setting the NumberList property of the [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement) class adds bullets.
1. The [ParagraphStyle](https://apireference.aspose.com/note/net/aspose.note/paragraphstyle) class defines the text formatting.
1. Generate the OneNote document by calling the Save method of the [Document](https://apireference.aspose.com/note/net/aspose.note/document) object.

The following code example demonstrates how to apply a bullet on the OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-ApplyNumberingOnText-ApplyNumberingOnText.cs" >}}
## **Insert Chinese Number List in the OneNote Document**
[Aspose.Note for .NET APIs](https://products.aspose.com/note/net) support inserting the Chinese number list in the OneNote document.

Aspose.Note for .NET offers the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents the OneNote file. Inserting the Chinese number list to the OneNote document page involves creating an [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement), which offers NumberList property to define the bullet.

Please see a brief description to add and apply bullets on the text in OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents the OneNote document.
1. Initialize three objects of [Page](https://apireference.aspose.com/note/net/aspose.note/page) class and set their levels.
1. Initialize the objects of [Outline](https://apireference.aspose.com/note/net/aspose.note/outline), [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement), and [RichText](https://apireference.aspose.com/note/net/aspose.note/richtext) classes. 
   Setting the NumberList property with Chinese counting format of the [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement) class adds bullets.
1. The [ParagraphStyle](https://apireference.aspose.com/note/net/aspose.note/paragraphstyle) class defines the text formatting.
1. Generate the OneNote document by calling the Save method of the [Document](https://apireference.aspose.com/note/net/aspose.note/document) object.

The following code example demonstrates how to apply a bullet on the OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-InsertChineseNumberList-InsertChineseNumberList.cs" >}}
## **Creating Page Title in MS OneNote Style**
Aspose.Note for .NET allows creating a page tile in default MS OneNote Style. The DefaultMsOneNoteTitleTextStyle property of the TextStyle class can be used to set the page title for this purpose.
### **Setting Page Title in Microsoft OneNote Style**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-CreateTitleMsStyle-CreateTitleMsStyle.cs" >}}
