---
title: Work, Extract, Insert Tables in OneNote Document using C#
linktitle: Working with Tables
type: docs
weight: 90
url: /net/working-with-tables/
description: OneNote C# API can be used to extract plain text from table or cell from row, insert table in OneNote Document and set cell background color.
---

## **Extracting Plain Text from the Table of OneNote Document**
[Aspose.Note for .NET](https://products.aspose.com/note/net/) allows developers to extract text from the entire table, a row or a particular cell element.

Aspose.Note for .NET offers the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents a OneNote file. The Document class exposes the GetChildNodes method that can be called to extract table nodes from a OneNote document.
### **Get Table Text from OneNote Document**
This example works as follows:

1. Create an object of the Document class.
1. Call the Document class' GetChildNodes method.
1. Retrieve a list of table nodes.
1. Call the LINQ-based Code to extract text
1. Display text on the output screen.

The following code example demonstrates how to get table text from a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Tables-ExtractTableText-ExtractTableText.cs" >}}
### **Get Row Text from a Table in a OneNote Document**
This example works as follows:

1. Create an object of the Document class.
1. Filter out a list of table nodes.
1. Iterate through table rows.
1. Call the LINQ-based Code to extract text.
1. Display the text on the output screen.

The following code example demonstrates how to extract row text from a table in a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Tables-ExtractRowText-ExtractRowText.cs" >}}
### **Get Cell Text from a Row in a Table**
This example works as follows:

1. Create an object of the Document class.
1. Filter out a list of table nodes.
1. Iterate through the table rows.
1. Filter out a list of cell nodes from each row.
1. Iterate through the row cells.
1. Call the LINQ-based Code to extract text.
1. Display the text on the output screen.

The following code example demonstrates how to get cell text from a row of the table.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Tables-ExtractCellText-ExtractCellText.cs" >}}
## **Insert a Table in OneNote Document**
Aspose.Note for .NET APIs allows developers to insert a table at the particular node position. This article is meant to show you how to create a table in OneNote document programmatically.

Aspose.Note for .NET offers the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents a OneNote file. Developers can append content under [TableCell](https://apireference.aspose.com/note/net/aspose.note/tablecell) node, table cells to the [TableRow](https://apireference.aspose.com/note/net/aspose.note/tablerow) node, table row to the [Table](https://apireference.aspose.com/note/net/aspose.note/table) node. Later they could append table under [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement) node, outline element to [Outline](https://apireference.aspose.com/note/net/aspose.note/outline) node, outline to [Page](https://apireference.aspose.com/note/net/aspose.note/page) node and then a page to the Document node. It's all based on the **Aspose.Note DOM structure**.

The following code example demonstrates how to insert a table in a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Tables-InsertTable-InsertTable.cs" >}}
## **Create a Table with Locked Columns in the OneNote Document**
Aspose.Note for .NET APIs allows developers to insert a table at the particular node position. This article is meant to show you how to create a table with a locked column in OneNote document programmatically.

Aspose.Note for .NET offers the [Document](https://apireference.aspose.com/note/net/aspose.note/document) class that represents a OneNote file. Developers can append content under [TableCell](https://apireference.aspose.com/note/net/aspose.note/tablecell) node, table cells to the [TableRow](https://apireference.aspose.com/note/net/aspose.note/tablerow) node, table row to the [Table](https://apireference.aspose.com/note/net/aspose.note/table) node. LockedWidth property of the Table class allows to bolt its width. Later they could append table under [OutlineElement](https://apireference.aspose.com/note/net/aspose.note/outlineelement) node, outline element to [Outline](https://apireference.aspose.com/note/net/aspose.note/outline) node, outline to [Page](https://apireference.aspose.com/note/net/aspose.note/page) node and then a page to the Document node. It's all based on the **Aspose.Note DOM structure**.

The following code example demonstrates how to insert a table with locked columns in a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Tables-CreateTableWithLockedColumns-CreateTableWithLockedColumns.cs" >}}
## **GetOutlineElementWithText Method**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Tables-InsertTable-GetOutlineElementWithText.cs" >}}
## **Setting Cell Background Color**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Tables-SettingCellBackGroundColor-SettingCellBackGroundColor.cs" >}}
## **Changing style of a table**
{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Tables-ChangeTableStyle.cs-ChangeTableStyle" >}}
![todo:image_alt_text](ChangeTableStyle.png)
