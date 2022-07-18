---
title: Working with Text Styles
type: docs
weight: 120
url: /java/working-with-text-styles/
---

## **Change the Font Color, Size and Highlight All the Text of RichText Node**
{{% alert color="primary" %}} 

This topic discusses changing the font color, size and highlighting all the text of a RichText node. This feature provides more in-depth control of OneNote to developers. Using this feature, developers can customize the font color, size and highlight text of any desired rich text node.

{{% /alert %}} 
### **Changing the Font Color, Size & Highlighting the Text**
To change the font and color of a rich text node using Aspose.Note, please follow the steps below:

1. Load OneNote document to a [Document](https://reference.aspose.com/note/java/com.aspose.note/Document) class.
1. Access a RichText node whose font and colors are to be changed.
1. Access TextStyle.
1. Set the text's font and color.

The output of the code snippet below is shown in the figure.

![todo:image_alt_text](working-with-text-styles_1.png)

### **Change style of the paragraph.**
{{< gist "aspose-com-gists" "952261680cb5075c778c0ae67a69bd14" "Examples-src-main-java-com-aspose-note-examples-styles-ChangeTextStyle-ChangeTextStyle.java" >}}
### **Set default paragraph style settings.**
{{< gist "aspose-note-gists" "0cd64f0457fdd6d56a68993a62169500" "src-main-java-com-aspose-note-examples-styles-SetDefaultParagraphStyle.java" >}}

The output file looks like:
![todo:image_alt_text](SetDefaultParagraphStyle.png)

### **Set proofing language for a text.**
{{< gist "aspose-note-gists" "0cd64f0457fdd6d56a68993a62169500" "src-main-java-com-aspose-note-examples-text-SetProofingLanguageForText.java" >}}

The output file looks like:
![todo:image_alt_text](SetProofingLanguageForText.png)
