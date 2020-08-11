---
title: Working with OneNote Document
type: docs
weight: 20
url: /net/working-with-onenote-document/
---

## **Extract OneNote Content using DocumentVisitor**
Aspose.Note can be used to parse Microsoft Office OneNote documents to extract separate document elements such as pages, images, rich text, outline, title, table, attached files, and others. Another possible task is to find all text and get a total count of nodes etc.

Use the [DocumentVisitor](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.DocumentVisitor+Class&linkCreation=true&fromPageId=19104346) class to implement this usage scenario. This class corresponds to the well-known Visitor design pattern. With DocumentVisitor, you can define and execute custom operations that require enumeration over the document tree.

DocumentVisitor provides a set of VisitXXX methods that are invoked when a particular document element (node) is encountered. For example, [DocumentVisitor.VisitRichTextStart](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.DocumentVisitor.VisitRichTextStart+Method&linkCreation=true&fromPageId=19104346) is called when the text item starts and [DocumentVisitor.VisitImageEnd](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.DocumentVisitor.VisitImageEnd+Method&linkCreation=true&fromPageId=19104346) is called when the visitor has visited all the children nodes. Each DocumentVisitor.VisitXXX method accepts the corresponding object that it encounters so you can use it as needed.

These are the steps you should follow to programmatically determine and extract various parts of a document:

1. Create a class derived from DocumentVisitor.
1. Override and provide implementations for some or all of the DocumentVisitor.VisitXXX methods to perform custom operations.
1. Call [Node.Accept](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Node.Accept+Method&linkCreation=true&fromPageId=19104346) on the node from where you want to start the enumeration. For example, if you want to enumerate the whole document, use [Document.Accept](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document.Accept+Method&linkCreation=true&fromPageId=19104346).

DocumentVisitor provides default implementations for all of the DocumentVisitor.VisitXXX methods. This makes it easier to create new document visitors as only the methods required for the particular visitor need to be overridden. It is not necessary to override all of the visitor methods.

The following code example demonstrates how to use the Visitor pattern to add new operations to the Aspose.Note object model. In this case, we create a simple document converter into a text format.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-ExtractContent-ExtractContent.cs" >}}
## **Aspose.Note Document Object Model**
### **Node Classes**
When Aspose.Note reads a OneNote document into memory, objects of different types are created to represent various document elements. Every RichText of text, title, table, and even the OneNote itself is a node. Aspose.Note defines a class for every type of document node.

The following illustration is a UML class diagram that shows inheritance between node classes of the Aspose.Note Document Object Model (DOM). The names of abstract classes are Node and CompositeNode. Please note that the Aspose.Note DOM also contains non-node classes such as [TextStyle](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TextStyle+Class&linkCreation=true&fromPageId=19104346), [Margins](http://www.aspose.com/api//net/note/aspose.note/margins), [NumberList](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.NumberList+Class&linkCreation=true&fromPageId=19104346)**,** etc that do not participate in the inheritance and they are not shown on this diagram.

{{% alert color="primary" %}} 

The following table lists Aspose.Note node classes and their short descriptions.

{{% /alert %}} 

|**Aspose.Note Class**|**Category**|**Description**|
| :- | :- | :- |
|[Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104346)|Document|A document object that, as the root of the document tree, provides access to the entire OneNote document.|
|[Title](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Title+Class&linkCreation=true&fromPageId=19104346)|Title|A page title of OneNote document.|
|[Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104346)|Page|A page of OneNote document.|
|[AttachedFile](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.AttachedFile+Class&linkCreation=true&fromPageId=19104346)|File|Represents an attached file within the OneNote document.|
|[Image](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Image+Class&linkCreation=true&fromPageId=19104346)|Image|Represents an image file within the OneNote document.|
|[OutlineGroup](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineGroup+Class&linkCreation=true&fromPageId=19104346)|Outline|Represents a group of outlines.|
|[OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104346)|Outline|Represents an outline element.|
|[Outline](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Outline+Class&linkCreation=true&fromPageId=19104346)|Outline|Represents an outline.|
|[Table](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Table+Class&linkCreation=true&fromPageId=19104346)|Tables|A table in a OneNote document.|
|[TableCell](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TableCell+Class&linkCreation=true&fromPageId=19104346)|Tables|A cell of a table row.|
|[TableRow](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TableRow+Class&linkCreation=true&fromPageId=19104346)|Tables|A row of a table.|
|[RichText](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.RichText+Class&linkCreation=true&fromPageId=19104346)|Text|A RichText of text with consistent formatting.|
The following table lists Aspose.Note base node classes that help to form the class hierarchy.

|**Class**|**Description**|
| :- | :- |
|[Node](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Node+Class&linkCreation=true&fromPageId=19104346)|Abstract base class for all nodes of a OneNote document. Provides basic functionality of a child node.|
|[CompositeNode](http://www.aspose.com/api//net/note/aspose.note.compositenode/1)|Base class for nodes that can contain other nodes. Provides operations to access, insert, remove and select child nodes.|
#### **Distinguish Nodes by NodeType**
Although the class of the node is sufficient enough to distinguish different nodes from each other, Aspose.Note provides the NodeType enumeration to simplify some API tasks such as selecting nodes of a specific type. The type of each node can be obtained using the [NodeType ](http://www.aspose.com/api/net/note/aspose.note/nodetype)enumeration. This returns a **NodeType** enumeration value. For example, a RichText node (represented by the **RichText *class) returns [NodeType.RichText](http://www.aspose.com/api/net/note/aspose.note/nodetype), a table node (represented by the {**}Table{*} class) returns [NodeType.Table](http://www.aspose.com/api/net/note/aspose.note/nodetype), and so on.

The following code example demonstrates how to use the NodeType enumeration.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-NodeTypeEnumeration-NodeTypeEnumeration.cs" >}}
## **Create an Empty OneNote Document with a Page Title**
Aspose.Note for .NET supports generating OneNote documents from scratch.

Use the code snippet given below to create a new document with a title.

This example work as follows:

1. Create an object of the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104346) class.
1. Initialize Page class object by passing the Document class object.
1. Set Page.Title object properties.
1. Call Document class' AppendChild method and pass Page class object.
1. Finally, save it by calling the Save method of Document class.

The following code snippet demonstrates how to create an empty OneNote document with a page title

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-CreateDocWithPageTitle-CreateDocWithPageTitle.cs" >}}
## **Getting File Format Information**
Aspose.Note API supports Microsoft OneNote as well as on OneNote online file formats. The lateral has some limitations such as no support for attachments and images in the document is not available. In order to guide the users about these two different types of documents, the API provides the method to determine the file format of the OneNote document so as to know the limitations until these are fully supported.

The following code example demonstrates how to retrieve the file format information of the OneNote document using the FileFormat property of the Document class.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Loading-and-Saving-RetreivingFileFormat-RetreivingFileFormat.cs" >}}
