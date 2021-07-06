---
title: Licensing
type: docs
weight: 50
url: /net/licensing/
---

## **Evaluation Version Limitations**
A free evaluation version of Aspose.Note for .NET can be downloaded from the downloads section of Aspose's web site at: <http://www.aspose.com/community/files/51/.net-components/aspose.note-for-.net/default.aspx>.
### **Limitation**
The evaluation version provides all the features except the following:

|**Usage context**|**Restrictions**|
| :- | :- |
|Opened MS OneNote document |Evaluation watermark is placed at the top of each page. First page has two full latest version of the page(current revision and one archive). Each another page has title with body replaced by evaluation watermark. Text elements are cut to 140 characters. Every third text element are replaced by watermark. Table elements are cut to three-by-three size. Image elements which exceed the limit of 500Kb are modified by writing evaluation message over the image. Every second image is erased.|
|Created MS OneNote document |Evaluation watermark is placed at the top of each page. First page шы saved including body's content. The body of each another page is replaced by evaluation watermark. Image elements which exceed the limit of 500Kb are modified by writing evaluation message over the image. Every second image is erased.|
|Opened/Created MS OneNote notebook |The number of the sections is restricted to two. The content of the rest of the sections are replaced by one empty page with evaluation watermark at the top. |
|Export MS OneNote to PDF |Evaluation watermark is placed at the top of each page of PDF file. The body of each page except the first one is deleted.|
|Export MS OneNote to image file |Evaluation watermark is placed at the top of an image.|
{{% alert color="primary" %}} 

If you want to try Aspose.Note without evaluation limitations, request a 30 day temporary license. Please refer to [How to get a Temporary License?](http://www.aspose.com/corporate/purchase/faqs/temporary-license.aspx) For more information.

{{% /alert %}} 
## **Other Limitations**
- Please note that you cannot set values against the **Application** and **Producer** fields while converting documents to PDF, because Aspose Ltd. and Aspose.Note for .NET x.x will be displayed against these fields.
## **Apply License using File or Stream Object**
The license can be loaded from a file or stream object. Aspose.Note for .NET will try to find the license in the following locations:

1. Explicit path.
1. The folder that contains Aspose.Note.dll.
1. The folder that contains the assembly that called Aspose.Note.dll.
1. The folder that contains the entry assembly (your .exe).
1. An embedded resource in the assembly that called Aspose.Note.dll.

The easiest way to set a license is to put the license file in the same folder as the Aspose.Note.dll file and specify the file name, without a path, as shown in the example below.

If you are using any other Aspose for .NET API along with Aspose.Note for .NET, please specify the namespace for the license like Aspose.Note.License.
### **Loading a License from File**
The easiest way to apply a license is to put the license file in the same folder as the Aspose.Note.dll file and specify just the file name without a path.

{{% alert color="primary" %}} 

When you call the SetLicense method, the license name that you pass should be that of the license file. For example, if you change the license file name to "Aspose.Note.lic.xml" pass that file name to the Note.SetLicense(…) method.

{{% /alert %}} 

{{< gist "aspose-note" "a3f450d09a204d8da28204807872cdcf" "Examples-CSharp-ApplyLicense-ApplyLicenseByPath-ApplyLicenseByPath.cs" >}}
### **Loading a License from a Stream Object**
The following example shows how to load a license from a stream.



{{< gist "aspose-note" "a3f450d09a204d8da28204807872cdcf" "Examples-CSharp-ApplyLicense-ApplyLicenseUsingFileStream-ApplyLicenseUsingFileStream.cs" >}}
## **Apply License using Embedded Resource**
One way of applying a license is to set it using a file or stream object. Another neat way of packaging the license with your application and making sure it will not be lost is to include it as an embedded resource into one of the assemblies that calls the component's DLL (included in Aspose.Note).

To include the license file as an embedded resource:

1. In Visual Studio .NET, include the license (.lic) file into the project by selecting **File**, then **Add Existing Item** and finally **Add**.
1. Select the file in the Solution Explorer.
1. Set the **Build Action** to **Embedded Resource** in the Properties window.
1. To access the license embedded in the assembly (as an embedded resource), just add the license file as an embedded resource to the project and pass the name of the license file to the SetLicense method. The License class automatically finds the license file in the embedded resources. There's no need to call the GetExecutingAssembly and GetManifestResourceStream methods of the System.Reflection.Assembly class in the Microsoft .NET Framework.

The example below illustrated this method of applying a license.



{{< gist "aspose-note" "a3f450d09a204d8da28204807872cdcf" "Examples-CSharp-ApplyLicense-ApplyLicenseByEmbeddedResource-ApplyLicenseByEmbeddedResource.cs" >}}
