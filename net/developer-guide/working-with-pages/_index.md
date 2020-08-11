---
title: Working with Pages
type: docs
weight: 60
url: /net/working-with-pages/
---

## **Get Number of Pages from the OneNote Document**
Aspose.Note for .NET supports retrieving the number of pages from a OneNote document.

This example works as follows:

1. Create an object of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104378) class.
1. Call Document class' GetChildNodes method.
1. Get a list of page nodes.
1. Get the number of pages via Count property.
1. Display the count on the output screen.

The following code snippet demonstrates how to get the number of pages from a OneNote file

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Pages-GetNumberOfPages-GetNumberOfPages.cs" >}}
## **Get Information of Each Page from the OneNote Document**
The [Page](http://www.aspose.com/api//net/note/aspose.note/page) class provides all the properties related to a page of a OneNote document. All the pages of the OneNote file are contained by page nodes of the [Document](http://www.aspose.com/api//net/note/aspose.note/document) object.

The following code example demonstrates how to get information about each page in a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Pages-GetPageInformation-GetPageInformation.cs" >}}
## **Create a OneNote Document with Root and Sub Level Pages**
This topic explains how developers can generate OneNote document including various pages at root or sub-level positions. Aspose.Note APIs lets the developer to programmatically choose the level of the page.
### **Generating Root and Sub Level Pages in OneNote**
Please see a brief description to create a OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104378) class that represents a OneNote document.
1. Initialize three objects of [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104378) class and set their levels.
1. Initialize separate objects of [Outline](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Outline+Class&linkCreation=true&fromPageId=19104378), [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104378), and [RichText](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.RichText+Class&linkCreation=true&fromPageId=19104378) classes for each [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104378) object by passing the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104378) class object. 
   Calling the AppendChild method of the [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104378), [Outline](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Outline+Class&linkCreation=true&fromPageId=19104378), [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104378), and [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104378) classes adds an appropriate new node that can be further used to add other nodes to the OneNote document.
1. The [TextStyle](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TextStyle+Class&linkCreation=true&fromPageId=19104378) class defines the text formatting.
1. Generate the OneNote document by calling the Save method of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104378) object.



{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Pages-CreateDocWithRootAndSubPages-CreateDocWithRootAndSubPages.cs" >}}
## **Working with Page Revision Information**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Pages-WorkingWithPageRevisions-WorkingWithPageRevisions.cs" >}}
## **Working with Page History**
### **Get All Revisions of a Specific Page**
Aspose.Note for .NET APIs provide support to get the history of a specific [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104378), e.g. how many times a page is updated, content tracking changes, and much more. All the pages of the OneNote file are contained by page nodes of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104378) object.

{{% alert color="primary" %}} 

There is a LoadHistory property of the [LoadOptions](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.LoadOptions+Class&linkCreation=true&fromPageId=19104378) class which tells whether the document loader should read and parse entire document history. The default value is true.

**In the case of a file with a huge amount of history, data consider using LoadHistory=false, to decrease memory and CPU usage.**

{{% /alert %}} 

The following code example demonstrates how to get a particular Page and then get its history revisions detail.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Pages-GetPageRevisions-GetPageRevisions.cs" >}}
### **Roll Back to Previous Page Version**
In order to roll back to a previous page version, the latest page needs to be removed from the document and the one before this one needs to be restored to the document as shown in the following code sample.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Pages-RollBackRevisions-RollBackRevisions.cs" >}}
### **Push Current Page Version to History**
The current page can be added to history by cloning it using the Page.Clone method.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Pages-PushCurrentPageVersion-PushCurrentPageVersion.cs" >}}
### **Modify Page History**
The current page can be added to history by cloning it using the Page.Clone method.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Pages-ModifyPageHistory-ModifyPageHistory.cs" >}}
## **Working with Conflict Pages**
A document can have pages with conflict pages in its history. Such pages are not saved to document by default. Aspose.Note API lets you manipulate such a page history using the IsConflictPage property of history page as shown below.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Pages-ConflictPageManipulation-ConflictPageManipulation.cs" >}}
## **Cloning Page with History**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Pages-PageClone-PageClone.cs" >}}
