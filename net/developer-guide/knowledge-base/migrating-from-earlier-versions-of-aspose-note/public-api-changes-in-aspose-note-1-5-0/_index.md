---
title: Public API Changes in Aspose.Note 1.5.0
type: docs
weight: 50
url: /net/public-api-changes-in-aspose-note-1-5-0/
---

{{% alert color="primary" %}} 

This document describes changes to the Aspose.Note API from version 1.4 to 1.5, that may be of interest to module/application developers. It includes not only new and updated public methods, but also a description of any changes in the behavior behind the scenes in Aspose.Note.

{{% /alert %}} 
## **Added new interfaces for child nodes**
The new interfaces for child nodes are added, e.g. INode, ICompositeNode, IOutlineElementChildNode, IOutlineChildNode and IPageChildNode etc. Almost all composite nodes now have a more strict type of child nodes unlike the base type Node previously.
### **Section and PageSeries were removed**
All properties which correspond to the Section node were moved to the Document (CreationTime,Color,DisplayName,Guid). Pages from the PageSeries node moved to the document's children and are accessible through the IEnumerable interface implemented by the Document type.
### **Added Page.Title property**
New Title property of the Page type was added to set page's title, unlike appending Title instance to the children collection.
### **CompositeNode was converted into a generic type**
To increase clarity of the OneNote composite node, old non-generic class was converted to a generic class with an interface INode constraint of the type parameter.
### **IsTitleText, IsTitleDate and IsTitleTime properties of the RichText type were marked as obsolete.**
The correct structure of Title's childrens contains RichText nodes for the title's text, date or time. Now these objects are accessible through TitleText, TitleDate and TitleTime properties respectively.
### **TableColumn.Ordinal was marked as obsolete.**
To specify an order for the columns the Table.Children property should be used.
### **Table.Rows was marked as obsolete.**
The property provides a read only list of rows. To change rows collection AppendChild and RemoveChild methods should be used.
### **RichText.IsTitleText was marked as obsolete.**
To set the text of the title Title.TitleText property should be used.
### **RichText.IsTitleDate was marked as obsolete.**
To set the date of the title Title.TitleDate property should be used.
### **RichText.IsTitleTime was marked as obsolete.**
To set the time of the title Title.TitleTime property should be used.
### **Image.Path was marked as obsolete.**
Use the constructor parameters to specify the path to the image.
### **Image.IsSizeSetByUser was marked as obsolete.**
The property does not affect anything.
### **NumberList.ctor() was marked as obsolete.**
Use other constructors to create a valid NumberList instance.
### **Image.ctor(Document document) was marked as obsolete.**
Use other constructors to create a valid Image instance.
