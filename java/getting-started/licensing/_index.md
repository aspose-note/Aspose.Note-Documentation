---
title: Licensing
description: A free evaluation version of Aspose.Note for Java (a Java API to interact with Microsoft Office OneNote programmatically without the software being installed on the server) can be downloaded from the downloads section of Aspose's web site. 
type: docs
weight: 30
url: /java/licensing/
---

## **Evaluation Version Limitations**
You can download Aspose.Note for Java free for evaluation. The evaluation version provides almost all functionality of the product with certain limitations. The same evaluation version becomes licensed when you purchase a license and add a couple of lines of code to apply the license.
### **PDF Creator Information**
Please note that you cannot set values against the **Application** and **Producer** fields while converting documents to PDF, because Aspose Ltd. and Aspose.Note for Java x.x will be displayed against these fields
### **Limitations**
The evaluation version provides all the features except the following:

|**Usage context**|**Restrictions**|
| :- | :- |
|Opened MS OneNote document |Evaluation watermark is placed at the top of each page. History data are restricted to the maximum number of three revisions per accessible page (current revision and two archive). Text elements are cutted to 500 characters. Table elements are cutted to three-by-three size. Image elements which exeed the limit of 500Kb are replaced by evaluation message as an alternative text. |
|Created MS OneNote document |Evaluation watermark is placed at the top of the first two pages. The rest of the pages are deleted. Image elements which exeed the limit of 500Kb are replaced by evaluation message as an alternative text. |
|Opened/Created MS OneNote notebook |The number of the sections is restricted to two. The content of the rest of the sections are replaced by one empty page with evaluation watermark at the top. |
|Export MS OneNote to PDF |Evaluation watermark is placed at the top of the first two pages of PDF file. The rest of the pages are deleted. |
|Export MS OneNote to image file |Evaluation watermark is placed at the top of an image. |
{{% alert color="primary" %}} 

If you want to test **Aspose.Note** without evaluation version limitations, request a 30-day temporary license. Please refer to [How to get a Temporary License?](https://purchase.aspose.com/temporary-license) for more information.

{{% /alert %}} 
## **Apply License Using File or Stream Object**
You can download an evaluation version of **Aspose.Note** for Java from [its download page](https://downloads.aspose.com/note/java). The evaluation version provides absolutely the same capabilities as the licensed version of the product. Furthermore, evaluation version simply becomes licensed when you purchase a license and add a couple of lines of code to apply the license.

Once you are happy with your evaluation of **Aspose.Note**, you can [purchase a license](https://purchase.aspose.com/buy) at the Aspose website. Make yourself familiar with the different subscription types offered. If you have any questions, do not hesitate to contact the Aspose sales team.

Every Aspose license carries a one-year subscription for free upgrades to any new versions or fixes that come out during this time. Technical support is free and unlimited and provided both to licensed and evaluation users.

### **Setting a License**
The license is a plain text XML file that contains details such as the product name, number of developers it is licensed to, subscription expiry date and so on. The file is digitally signed, so do not modify the file; even the inadvertent addition of an extra line break into the file will invalidate it.

You need to set a license before utilizing Aspose.Note if you want to avoid its evaluation limitations. You are only required to set a license once per application or process.

The license can be loaded from a stream or file in the following locations:

1. Explicit path.
1. The folder that contains the Aspose.Note.jar.

Use the **License.setLicense()** method to license the component. Often the easiest way to set a license is to put the license file in the same folder as Aspose.Note.jar and specify just the file name without path as shown in the following example:
#### **Example 1**
In this example **Aspose.Note** will attempt to find the license file in the folder that contain the JARs of your application.

**Java**

{{< highlight csharp >}}

 com.aspose.note.License license = new com.aspose.note.License();

license.setLicense("Aspose.Note.Java.lic");

{{< /highlight >}}
#### **Example 2**
Initializes a license from a stream.

**Java**

{{< highlight csharp >}}

 com.aspose.note.License license = new com.aspose.note.License();

license.setLicense(new java.io.FileInputStream("Aspose.Note.Java.lic"));

{{< /highlight >}}
