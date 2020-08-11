---
title: Working with Attachments
type: docs
weight: 100
url: /net/working-with-attachments/
---

## **Retrieve Attached Files from a OneNote Document**
All files attached to a Microsoft OneNote document can be retrieved. These files are stored in AttachedFile nodes. The AttachedFile class represents an attached file.

To extract all attached files from a OneNote document, follow these steps:

1. Use the [Document](http://www.aspose.com/api/net/note/aspose.note/document).GetChildNodes method to select all AttachedFile nodes.
1. Iterate through the resulting node collections.
1. Extract image bytes array using the AttachedFile.Bytes property.
1. Save attached file bytes to local space.

The following code example demonstrates how to extract attached files from a OneNote document and save them to local space.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Attachments-RetrieveAttachedFiles-RetrieveAttachedFiles.cs" >}}

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Attachments-RetrieveAttachedFiles-CopyStream.cs" >}}
## **Attach a File to the OneNote Document**
To keep a copy of any document or file as part of the OneNote document, developers can attach it to OneNote page. The [AttachedFile](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.AttachedFile+Class&linkCreation=true&fromPageId=19104332) class represents an attachment file.

To attach a file to a OneNote document, follow these steps:

1. Use the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104332) class to generate the OneNote file.
1. Initialize [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104332), [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104332) and [Outline](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Outline+Class&linkCreation=true&fromPageId=19104332) classes by passing document object.
1. Initialize [AttachedFile](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.AttachedFile+Class&linkCreation=true&fromPageId=19104332) object by passing the document object and file path.
1. Add attached file node under OutlineElement node.
1. Save a OneNote document.
### **Attach File by Passing its Path**
The following code example demonstrates how to attach a file to a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Attachments-AttachFileByPath-AttachFileByPath.cs" >}}
### **Attach File and Set its Icon by Passing Files Path**
The following code example demonstrates how to attach a file and also set attach file icon in OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Attachments-AttachFileAndSetIcon-AttachFileAndSetIcon.cs" >}}