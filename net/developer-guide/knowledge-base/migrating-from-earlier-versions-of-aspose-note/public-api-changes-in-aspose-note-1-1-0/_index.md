---
title: Public API Changes in Aspose.Note 1.1.0
type: docs
weight: 10
url: /net/public-api-changes-in-aspose-note-1-1-0/
---

{{% alert color="primary" %}} 

This document describes changes to the Aspose.Note API from version 1.0 to 1.1, that may be of interest to module/application developers. It includes not only new and updated public methods, but also a description of any changes in the behavior behind the scenes in Aspose.Note.

{{% /alert %}} 
### **The INotebookVisitor Interface is now a DocumentVisitor Abstract Class**
Use DocumentVisitor class parsing OneNote documents in order to extract separate document elements such as Sections, Pages, Outlines, Group Outlines, images, and others.
### **The FirstChild, LastChild, NextSibling, and PreviousSibling methods are implemented**
Starting with this version of Aspose.Note, it is now possible to access:

1. PreviousSibling and NextSibling methods from the Aspose.Note.Node class.
1. PreviousSibling, NextSibling, FirstChild and LastChild methods from the Aspose.Note.CompositeNode class.
### **NumberFormat Enum Added**
Use the NumberFormat enumeration to distinguish each number. For now, it has a single constant: "DecimalNumbers".
### **NumberList Class Added**
The NumberList class helps accessing and manipulating bullet and numbered lists. Developers can also access list properties, such as font name, numbering format, and many others. Please see a complete example topic: [Retrieve Bullet or Number List Properties](https://docs.aspose.com/note/net/working-with-text/#retrieve-bullet-or-number-list-properties). 

The [OutlineElement class](https://apireference.aspose.com/note/net/aspose.note/outlineelement) exposes the [NumberList property](https://apireference.aspose.com/note/net/aspose.note/numberlist).
### **The SpaceBefore, SpaceAfter and LineSpacing Properties Implemented**
The SpaceBefore, SpaceAfter, and LineSpacing properties are added to the [RichText class](https://apireference.aspose.com/note/net/aspose.note/richtext). It allows you to get or set the minimum amount of space before the text line, get or set the minimum amount of space after the text line, and get or set line spacing respectively.
