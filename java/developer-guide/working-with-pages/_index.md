---
title: Working with Pages
type: docs
weight: 50
url: /java/working-with-pages/
---

{{% alert color="primary" %}} 

Aspose.Note for Java APIs provide support to get the history of a specific [Page](http://www.aspose.com/api/java/note/com.aspose.note/classes/Page), e.g. how many times a page is updated, content tracking changes and much more. All the pages of the OneNote file are contained by page nodes of the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) object.

{{% /alert %}} 
## **Get Number of Pages from the OneNote Document**
Aspose.Note for Java supports retrieving number of pages from a OneNote document.

This example work as follows:

1. Create an object of the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) class.
1. Call Document class' getChildNodes method.
1. Get a list of page nodes.
1. Get the number of pages via Count property.
1. Display the count on the output screen.

The following code snippet shows you how to get the number of pages from a OneNote file

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-pages-GetPageCount-GetPageCount.java" >}}
## **Get Information of Each Page from the OneNote Document**
The [Page](http://www.aspose.com/api/java/note/com.aspose.note/classes/Page) class provides all the properties related to a page of a OneNote document. All the pages of the OneNote file are contained by page nodes of the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) object.

The code below shows how to get information about each page in a OneNote document.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-pages-GetInfo-GetInfo.java" >}}
## **Create OneNote Document with Root and Sub Level Pages**
This article explains how developers can generate OneNote document including various pages at root or sub-level positions. Aspose.Note APIs lets the developer to programmatically choose the level of the page.
### **Generating Root and Sub Level Pages in OneNote**
Please see brief description to create a OneNote document using the Aspose.Note APIs:

1. Create an instance of the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) class that represents a OneNote document.
1. Initialize three objects of [Page](http://www.aspose.com/api/java/note/com.aspose.note/classes/Page) class and set their levels.
1. Initialize separate objects of [Outline](http://www.aspose.com/api/java/note/com.aspose.note/classes/Outline), [OutlineElement](http://www.aspose.com/api/java/note/com.aspose.note/classes/OutlineElement) and [RichText](http://www.aspose.com/api/java/note/com.aspose.note/classes/RichText) classes for each [Page](http://www.aspose.com/api/java/note/com.aspose.note/classes/Page) object by passing the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) class object. 
   Calling the AppendChildLast method of the [OutlineElement](http://www.aspose.com/api/java/note/com.aspose.note/classes/OutlineElement), [Outline](http://www.aspose.com/api/java/note/com.aspose.note/classes/Outline), [Page](http://www.aspose.com/api/java/note/com.aspose.note/classes/Page) and [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) classes adds an appropriate new node that can be further used to add other nodes to the OneNote document.
1. The [TextStyle](http://www.aspose.com/api/java/note/com.aspose.note/classes/TextStyle) class defines the text formatting.
1. Generate the OneNote document by calling the Save method of the [Document](http://www.aspose.com/api/java/note/com.aspose.note/classes/Document) object.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-pages-CreateDocWithRootAndSubPages-CreateDocWithRootAndSubPages.java" >}}
## **Working with Page Revision Information**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-pages-WorkingWithPageRevisions-WorkingWithPageRevisions.java" >}}
## **Working with Page History**
### **Get All Revisions of a Specific Page**
There is a LoadHistory property of the [LoadOptions](http://www.aspose.com/api/java/note/com.aspose.note/classes/LoadOptions) class which tells whether the document loader should read and parse entire document history. The default value is true. **In case of file with huge amount of history data consider using LoadHistory=false, to decrease memory and CPU usage.**

The code sample below shows how to get a particular Page and then get its history revisions detail.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-pages-GetPageRevisions-GetPageRevisions.java" >}}
### **Roll Back To Previous Page Version**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-pages-RollBackToPreviousPageVersion-RollBackToPreviousPageVersion.java" >}}
### **Push Current Page Version To History**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-pages-PushCurrentPageVersion-PushCurrentPageVersion.java" >}}
### **Modify Page History**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-pages-ModifyPageHistory-ModifyPageHistory.java" >}}
## **Working with Conflict Pages**
A document can have pages with conflict pages in its history. Such pages are not saved to document by default. Aspose.Note API lets you manipulate such a page history using the isConflictPage method of history page as shown below.

{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-pages-ConflictPageManipulation-ConflictPageManipulation.java" >}}
