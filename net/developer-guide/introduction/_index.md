---
title: Introduction
type: docs
weight: 10
url: /net/introduction/
---

## **Create a Hello World OneNote document Using API**
This article explains how to create a OneNote document from scratch using the simple APIs provided by Aspose.Note for .NET. To create a OneNote document, add page, outline, outline element and text dynamically using the set of classes packaged in the [Aspose.Note](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note+namespace&linkCreation=true&fromPageId=19104337) namespace.

Please follow these steps to create a OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104337) class that represents a OneNote document.
1. If you have purchased a license, then embed the code to apply for that license with the help of the [License](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.License+Class&linkCreation=true&fromPageId=19104337) class.
1. Initialize one object of [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104337), [Outline](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Outline+Class&linkCreation=true&fromPageId=19104337), [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104337) and [RichText](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.RichText+Class&linkCreation=true&fromPageId=19104337) classes bypassing the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104337) class object. 
   Calling the AppendChild method of the [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104337), [Outline](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Outline+Class&linkCreation=true&fromPageId=19104337), [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104337) and [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104337) classes adds an appropriate new node that can be further used to add new nodes to the OneNote document.
1. The [TextStyle](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TextStyle+Class&linkCreation=true&fromPageId=19104337) class defines the text formatting. Similarly, the DefaultStyle property exposed by [RichText](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.RichText+Class&linkCreation=true&fromPageId=19104337) class allows applying to format on the text.
1. Generate the OneNote document by calling the Save method of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104337) object.
### **Create a OneNote Document with Simple RichText**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-CreateDocWithSimpleRichText-CreateDocWithSimpleRichText.cs" >}}
### **Create a OneNote Document with Formatted RichText**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-CreateDocWithFormattedRichText-CreateDocWithFormattedRichText.cs" >}}
