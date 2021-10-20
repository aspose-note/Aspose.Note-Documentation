---
title: Basic samples how to convert OneNote to Html
type: docs
weight: 30
url: /net/convert-onenote-to-html/basic-samples/
---

### **Save OneNote to Html using default options**

The following code example demonstrates how to convert OneNote to Html using the default options.
With default options all pages of the document are saved, css and images are saved to separate files and fonts are not exported.

{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Loading-and-Saving-CreateOneNoteDocAndSaveToHTML.cs-CreateAndSaveToHTMLUsingDefaultOptions" >}}


### **Save specified page's range of OneNote to Html**

The following code example demonstrates how to convert a specified range of pages from OneNote to Html. This range is specified by setting PageIndex and PageCount properties.

The code below saves the first page of OneNote document into a file in HTML format.
             
{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Loading-and-Saving-CreateOneNoteDocAndSaveToHTML.cs-CreateAndSavePageRange" >}}


### **Save OneNote to Html with embedded resources**

Html/CSS allows to store inside all required resources(fonts/images/css).
The following code example demonstrates how to convert OneNote to Html with embedding of all resources(css/fonts/images).
             
{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Loading-and-Saving-CreateOneNoteDocAndSaveToHTML.cs-SaveAsHTMLToMemoryStreamWithEmbeddedResources" >}}


### **Save OneNote to Html with resources in separate files**

The default way to store resources like fonts/images/css is external files.
The following code example demonstrates how to convert OneNote to Html with storing all resources(css/fonts/images) to a separate files.
             
{{< gist "aspose-note-gists" "ea99b163e8b22eca0473e9be10c83d7c" "Examples-CSharp-Loading-and-Saving-CreateOneNoteDocAndSaveToHTML.cs-SaveAsHTMLToFileWithResourcesInSeparateFiles" >}}
