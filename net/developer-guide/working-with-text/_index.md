---
title: Working with Text
type: docs
weight: 80
url: /net/working-with-text/
---

## **Extract Text from OneNote Document**
One of the tasks that developers need to perform is extracting text from an OneNote document. [Aspose.Note for .NET](http://www.aspose.com/.net/onenote-component.aspx) allows developers to extract text from OneNote document in various ways.

Aspose.Note for .NET offers the [Document](http://www.aspose.com/api/net/note/aspose.note/document) class that represents the OneNote file. The simple LINQ can be used to extract text from the OneNote document.
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
Aspose.Note for .NET supports finding and then replacing text within OneNote document. Aspose.Note for .NET offers the [Document](http://www.aspose.com/api/net/note/aspose.note/document) class that represents the OneNote file.
### **Replace Text on All Pages**
The following code example demonstrates how to replace text on all pages.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-ReplaceTextOnAllPages-ReplaceTextOnAllPages.cs" >}}
### **Replace Text on a Particular Page**
The following code example demonstrates how to replace text on a particular page.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-ReplaceTextOnParticularPage-ReplaceTextOnParticularPage.cs" >}}
## **Retrieve Bullet or Number List Properties**
[Aspose.Note for .NET](http://www.aspose.com/.net/onenote-component.aspx) provides comprehensive support for Microsoft OneNote lists. Developers can access a number of list properties, such as font name, numbering format, and many others.
### **Retrieving Properties**
Aspose.Note for .NET offers the [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104386) class that represents an outline inside a OneNote document. The OutlineElement class exposes the NumberList property that can be called to extract bullet or numbered list properties. The following example shows how to extract bullet or numbered list properties from a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-RetrieveBulletOrNumberList-RetrieveBulletOrNumberList.cs" >}}
## **Apply Bullets on the Text**
Arranging texts in bullet form is a very common approach. Aspose.Note for .NET APIs allows developers to arrange text items in bullets.

Aspose.Note for .NET offers the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104386) class that represents a OneNote file. Writing text to a OneNote document page involves creating an [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104386), which offers NumberList property to define the bullet.

Please see brief description to add and apply bullets on the text in OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104386) class that represents a OneNote document.
1. Initialize three objects of [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104386) class and set their levels.
1. Initialize the objects of [Outline](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Outline+Class&linkCreation=true&fromPageId=19104386), [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104386) and [RichText](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.RichText+Class&linkCreation=true&fromPageId=19104386) classes. 
   Setting the NumberList property of the [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104386) class adds bullets.
1. The [TextStyle](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TextStyle+Class&linkCreation=true&fromPageId=19104386) class defines the text formatting.
1. Generate the OneNote document by calling the Save method of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104386) object.

The following code example demonstrates how to apply a bullet on the OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-ApplyBulletsOnText-ApplyBulletsOnText.cs" >}}
## **Apply Numbering on the Text**
Arranging texts in numbering form is a very common approach. Aspose.Note for .NET APIs allows developers to arrange text items in numbering.

Aspose.Note for .NET offers the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104386) class that represents a OneNote file. Writing text to a OneNote document page involves creating an [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104386), which offers NumberList property to define the bullet.

Please see brief description to add and apply bullets on the text in OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104386) class that represents a OneNote document.
1. Initialize three objects of [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104386) class and set their levels.
1. Initialize the objects of [Outline](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Outline+Class&linkCreation=true&fromPageId=19104386), [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104386) and [RichText](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.RichText+Class&linkCreation=true&fromPageId=19104386) classes. 
   Setting the NumberList property of the [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104386) class adds bullets.
1. The [TextStyle](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TextStyle+Class&linkCreation=true&fromPageId=19104386) class defines the text formatting.
1. Generate the OneNote document by calling the Save method of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104386) object.

The following code example demonstrates how to apply a bullet on the OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-ApplyNumberingOnText-ApplyNumberingOnText.cs" >}}
## **Insert Chinese Number List in the OneNote Document**
[Aspose.Note for .NET APIs](http://www.aspose.com/.net/onenote-component.aspx) support inserting Chinese number list in the OneNote document.

Aspose.Note for .NET offers the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104386) class that represents the OneNote file. Inserting the Chinese number list to OneNote document page involves creating an [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104386), which offers NumberList property to define the bullet.

Please see a brief description to add and apply bullets on the text in OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104386) class that represents the OneNote document.
1. Initialize three objects of [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104386) class and set their levels.
1. Initialize the objects of [Outline](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Outline+Class&linkCreation=true&fromPageId=19104386), [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104386), and [RichText](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.RichText+Class&linkCreation=true&fromPageId=19104386) classes. 
   Setting the NumberList property with Chinese counting format of the [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104386) class adds bullets.
1. The [TextStyle](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TextStyle+Class&linkCreation=true&fromPageId=19104386) class defines the text formatting.
1. Generate the OneNote document by calling the Save method of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104386) object.

The following code example demonstrates how to apply a bullet on the OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-InsertChineseNumberList-InsertChineseNumberList.cs" >}}
## **Creating Page Title in MS OneNote Style**
Aspose.Note for .NET allows creating a page tile in default MS OneNote Style. The DefaultMsOneNoteTitleTextStyle property of the TextStyle class can be used to set the page title for this purpose.
### **Setting Page Title in Microsoft OneNote Style**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-CreateTitleMsStyle-CreateTitleMsStyle.cs" >}}
