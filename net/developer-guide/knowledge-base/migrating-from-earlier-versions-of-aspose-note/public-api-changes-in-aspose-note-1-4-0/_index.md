---
title: Public API Changes in Aspose.Note 1.4.0
type: docs
weight: 40
url: /net/public-api-changes-in-aspose-note-1-4-0/
---

{{% alert color="primary" %}} 

This document describes changes to the Aspose.Note API from version 1.3 to 1.4, that may be of interest to module/application developers. It includes not only new and updated public methods, but also a description of any changes in the behavior behind the scenes in Aspose.Note.

{{% /alert %}} 
### **New Approach to Retrieve OneNote Document Nodes**
A new method for getting nodes by type was developed to provide a more flexible approach and avoid type casting.
Old sample code (.NET, C#):

**C#**

{{< highlight csharp >}}
 // load OneNote document
 Aspose.Note.Document oneFile = new Aspose.Note.Document(@"Test.one");
 
 // retrieve RichText type nodes
 IList<Node> richTextNodes = oneFile.GetChildNodes(Aspose.Note.NodeType.RichText);
 
 // retrieve a particular node from the collection
 Aspose.Note.RichText firstTextNode = (Aspose.Note.RichText)richTextNodes[0];
{{< /highlight >}}

New sample code (.NET, C#):

**C#**

{{< highlight csharp >}}
 // load OneNote document
 Aspose.Note.Document oneFile = new Aspose.Note.Document(@"Test.one");
 
 // retrieve RichText type nodes
 IList<RichText> richTextNodes = oneFile.GetChildNodes<RichText>();
 
 // retrieve a particular node from the collection
 Aspose.Note.RichText firstTextNode = richTextNodes[0];
{{< /highlight >}}
