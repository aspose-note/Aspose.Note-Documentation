---
title: Working with Text Styles
type: docs
weight: 130
url: /net/working-with-text-styles/
---

## **Change the Font Color, Size and Highlight All the Text of RichText Node**
This topic discusses changing the font color, size and highlighting all the text of a RichText node. This feature provides more in-depth control of OneNote to developers. Using this feature, developers can customize the font color, size and highlight text of any desired rich text node.

To change the font and color of a rich text node using Aspose.Note, please follow the steps below:

1. Load OneNote document to a [Document](https://reference.aspose.com/note/net/aspose.note/document) class.
1. Access a RichText node whose font and colors are to be changed.
1. Access TextStyle.
1. Set the text's font and color.

### **Change style of the paragraph**
{{< gist "aspose-com-gists" "f1c4460425d3a75dd63cd514a9833946" "Examples-CSharp-Text-ChangeStyle-ChangeStyle.cs" >}}

### **Set default paragraph style settings**
{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Text-SetDefaultParagraphStyle.cs" >}}

### **Set proofing language for a text**
{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Text-SetProofingLanguageForText.cs" >}}

### **Apply Dark mode style**

The following code example demonstrates how to make OneNote document to look like in Dark mode. 
             
{{< highlight csharp >}}
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{   
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
{{< /highlight >}}
