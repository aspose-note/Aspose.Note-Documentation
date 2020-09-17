---
title: Public API Changes in Aspose.Note 1.2.0
type: docs
weight: 20
url: /net/public-api-changes-in-aspose-note-1-2-0/
---

{{% alert color="primary" %}} 

This document describes changes to the Aspose.Note API from version 1.1 to 1.2, that may be of interest to module/application developers. It includes not only new and updated public methods, but also a description of any changes in the behavior behind the scenes in Aspose.Note.

{{% /alert %}} 
### **DocumentVisitor Abstract Class Now More Flexible**
A few more common OneNote document elements are supported. The DocumentVisitor class allows you to parse OneNote document elements such as NoteTag, TagIcon, Table, AttachedFile.DocumentVisitor class changes are as follows:

- The DocumentVisitor.VisitDocument method has been renamed to DocumentVisitor.VisitDocumentStart.
- The DocumentVisitor.VisitImage method has been renamed to DocumentVisitor.VisitImageStart.
- The DocumentVisitor.VisitOutline method has been renamed to DocumentVisitor.VisitOutlineStart.
- The DocumentVisitor.VisitOutlineElement method has been renamed to DocumentVisitor.VisitOutlineElementStart.
- The DocumentVisitor.VisitOutlineGroup method has been renamed to DocumentVisitor.VisitOutlineGroupStart.
- The DocumentVisitor.VisitPage method has been renamed to DocumentVisitor.VisitPageStart.
- The DocumentVisitor.VisitPageSeries method has been renamed to DocumentVisitor.VisitPageSeriesStart.
- The DocumentVisitor.VisitRichText method has been renamed to DocumentVisitor.VisitRichTextStart.
- The DocumentVisitor.VisitSection method has been renamed to DocumentVisitor.VisitSectionStart.
- The DocumentVisitor.VisitTitle method has been renamed to DocumentVisitor.VisitTitleStart.
- A few end methods have been added as DocumentVisitor.VisitDocumentEnd, DocumentVisitor.VisitImageEnd, DocumentVisitor.VisitOutlineEnd, DocumentVisitor.VisitOutlineElementEnd, DocumentVisitor.VisitOutlineGroupEnd, DocumentVisitor.VisitPageEnd, DocumentVisitor.VisitPageSeriesEnd, DocumentVisitor.VisitRichTextEnd, DocumentVisitor.VisitSectionEnd, DocumentVisitor.VisitTitleEnd, DocumentVisitor.VisitAttachedFileEnd, DocumentVisitor.VisitTableEnd, DocumentVisitor.VisitTableCellEnd, DocumentVisitor.VisitTableRowEnd. It calls after visitor visited the all children nodes.
### **Tag Notes are Supported**
Aspose.Note for .NET allows developers to programmatically access details about important tag notes. Also, tag notes will be rendered when exporting OneNote documents to any supported file format. Please see a complete example topic: [Get Note Tag Details from a OneNote Document](https://docs.aspose.com/note/net/working-with-tags/#get-note-tag-details-from-a-onenote-document)
### **Outlook Tasks are Supported**
Outlook tasks are being carried. Developers can now access and render them using the Aspose.Note API. Please have a look on this help example topic: [Get Outlook Task Details from a OneNote Document](https://docs.aspose.com/note/net/working-with-tasks/)
### **Tables are Supported**
The Aspose.Note API allows developers to export OneNote documents along with tables to any supported format. Developers can also access tables and their child elements. This example topic shows how to extract text from a table: [Extracting Plain Text from the Table of OneNote Document](https://docs.aspose.com/note/net/working-with-tables/#extracting-plain-text-from-the-table-of-onenote-document)
### **Attached Files are Supported**
All files attached to a OneNote document can be retrieved. Developers can easily find attached files after converting OneNote documents via the Aspose.Note. Please see the following topic for further help: [Retrieve Attached Files from a OneNote Document](https://docs.aspose.com/note/net/working-with-attachments/#retrieve-attached-files-from-a-onenote-document)
### **Hyperlinks Rendering is Supported**
Aspose.Note preserves hyperlinks when the OneNote document is converted to any supported format.