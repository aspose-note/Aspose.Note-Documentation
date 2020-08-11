---
title: Working with Tables
type: docs
weight: 90
url: /net/working-with-tables/
---

## **Extracting Plain Text from the Table of OneNote Document**
[Aspose.Note for .NET](http://www.aspose.com/.net/onenote-component.aspx) allows developers to extract text from the entire table, a row or a particular cell element.

Aspose.Note for .NET offers the [Document](http://www.aspose.com/api/net/note/aspose.note/document) class that represents a OneNote file. The Document class exposes the GetChildNodes method that can be called to extract table nodes from a OneNote document.
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
[Aspose.Note for .NET](http://www.aspose.com/.net/onenote-component.aspx) APIs allows developers to insert a table at particular node position. This article is meant to show you how to create a table in OneNote document programmatically.

Aspose.Note for .NET offers the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104320) class that represents a OneNote file. Developers can append content under [TableCell](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TableCell+Class&linkCreation=true&fromPageId=19104320) node, table cells to the [TableRow](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TableRow+Class&linkCreation=true&fromPageId=19104320) node, table row to the [Table](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Table+Class&linkCreation=true&fromPageId=19104320) node. Later they could append table under [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104320) node, outline element to [Outline](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Outline+Class&linkCreation=true&fromPageId=19104320) node, outline to [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104320) node and then a page to the Document node. It's all based on the **Aspose.Note DOM structure**.

The following code example demonstrates how to insert a table in a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Tables-InsertTable-InsertTable.cs" >}}
## **Create a Table with Locked Columns in the OneNote Document**
[Aspose.Note for .NET](http://www.aspose.com/.net/onenote-component.aspx) APIs allows developers to insert a table at particular node position. This article is meant to show you how to create a table with a locked column in OneNote document programmatically.

Aspose.Note for .NET offers the [Document](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Document+Class&linkCreation=true&fromPageId=19104320) class that represents a OneNote file. Developers can append content under [TableCell](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TableCell+Class&linkCreation=true&fromPageId=19104320) node, table cells to the [TableRow](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.TableRow+Class&linkCreation=true&fromPageId=19104320) node, table row to the [Table](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Table+Class&linkCreation=true&fromPageId=19104320) node. LockedWidth property of the Table class allows to bolt its width. Later they could append table under [OutlineElement](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.OutlineElement+Class&linkCreation=true&fromPageId=19104320) node, outline element to [Outline](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Outline+Class&linkCreation=true&fromPageId=19104320) node, outline to [Page](/pages/createpage.action?spaceKey=notenet&title=Aspose.Note.Page+Class&linkCreation=true&fromPageId=19104320) node and then a page to the Document node. It's all based on the **Aspose.Note DOM structure**.

The following code example demonstrates how to insert a table with locked columns in a OneNote document.

{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Tables-CreateTableWithLockedColumns-CreateTableWithLockedColumns.cs" >}}
## **Setting Cell Background Color**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Tables-SettingCellBackGroundColor-SettingCellBackGroundColor.cs" >}}
## **GetOutlineElementWithText Method**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Tables-InsertTable-GetOutlineElementWithText.cs" >}}
