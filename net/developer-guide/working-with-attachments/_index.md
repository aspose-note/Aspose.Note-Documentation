---
title: Working with Attachments
type: docs
weight: 100
url: /net/working-with-attachments/
---

## **Retrieve Attached Files from a OneNote Document**
All files attached to a Microsoft OneNote document can be retrieved. These files are stored in AttachedFile nodes. The AttachedFile class represents an attached file.

To extract all attached files from a OneNote document, follow these steps:

1. Use the [Document](https://apireference.aspose.com/note/net/aspose.note/document).GetChildNodes method to select all AttachedFile nodes.
1. Iterate through the resulting node collections.
1. Extract image bytes array using the AttachedFile.Bytes property.
1. Save the attached file bytes to the local space.

The following code example demonstrates how to extract attached files from a OneNote document and save them to local space.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Attachments-RetrieveAttachedFiles-RetrieveAttachedFiles.cs" >}}

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Attachments-RetrieveAttachedFiles-CopyStream.cs" >}}
## **Attach a File to the OneNote Document**
To keep a copy of any document or file as part of the OneNote document, developers can attach it to the OneNote page. The [AttachedFile](https://apireference.aspose.com/note/net/aspose.note/attachedfile) class represents an attachment file.

To attach a file to a OneNote document, follow these steps:

1. Use the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class to generate the OneNote file.
1. Initialize [Page](https://apireference.aspose.com/note/net/aspose.note/page), [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement) and [Outline](https://apireference.aspose.com/note/net/aspose.note/outline) classes by passing document object.
1. Initialize [AttachedFile](https://apireference.aspose.com/note/net/aspose.note/attachedfile) object by passing the document object and file path.
1. Add attached file node under the OutlineElement node.
1. Save a OneNote document.
### **Attach File by Passing its Path**
The following code example demonstrates how to attach a file to a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Attachments-AttachFileByPath-AttachFileByPath.cs" >}}
### **Attach File and Set its Icon by Passing Files Path**
The following code example demonstrates how to attach a file and also set attach file icon in the OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Attachments-AttachFileAndSetIcon-AttachFileAndSetIcon.cs" >}}
