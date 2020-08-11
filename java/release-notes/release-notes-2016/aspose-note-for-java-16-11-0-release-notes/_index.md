---
title: Aspose.Note for Java 16.11.0 Release Notes
type: docs
weight: 20
url: /java/aspose-note-for-java-16-11-0-release-notes/
---

Aspose.Note for Java is a class library that enables applications to interact with Microsoft Office OneNote programmatically without it being installed on the server. It is a pure alternate for the Microsoft OneNote Object Model and provides better performance and ease of use for managing OneNote documents.

Visit the documentation to learn how to [Getting Started](http://www.aspose.com/docs/display/notejava/Getting+Started).
### **Features and Improvements**

|**Key**|**Summary**|**Category**|
| :- | :- | :- |
|NOTEJAVA-35 |Support for creation of [password protected](http://www.aspose.com/docs/display/notejava/Save+a+OneNote+Document#SaveaOneNoteDocument-CreatingPasswordProtectedOneNoteDocuments) MS OneNote documents. |New Feature |
|NOTEJAVA-109 |Provide support of password protected documents ([reading](http://www.aspose.com/docs/display/notejava/Working+with+OneNote+Notebook#WorkingwithOneNoteNotebook-LoadingPasswordProtectedDocumentsasapartof.onetoc2Notebook) and [writing ](http://www.aspose.com/docs/display/notejava/Working+with+OneNote+Notebook#WorkingwithOneNoteNotebook-SupportofPasswordProtectedDocumentsWritingasPartof.onetoc2Notebook)) as a part of .onetoc2 notebook. |Enhancement |
|NOTEJAVA-205 |Notebook: Provide option to [load file from Stream](http://www.aspose.com/docs/display/notejava/Working+with+OneNote+Notebook#WorkingwithOneNoteNotebook-LoadingNotebookFilefromStream). |Enhancement |
|NOTEJAVA-206 |Provide option to [save Notebook to stream](http://www.aspose.com/docs/display/notejava/Working+with+OneNote+Notebook#WorkingwithOneNoteNotebook-SavingNotebooktoStream). |Enhancement |
|NOTEJAVA-40 |Add background [color property](http://www.aspose.com/docs/display/notejava/Working+with+Tables#WorkingwithTables-SettingCellBackgroundColor) for table cells. |Enhancement |
|NOTENET-2143 |Exception while loading OneNote Online file provided by user. |Bug |
|NOTENET-2145 |Failed to open OneNote document. |Bug |
|NOTENET-2156 |Broken pictures while opening documents that were password protected with MS OneNote. |Bug |
### **Public API and Backward Incompatible Changes**
The following public methods and properties were added.

|**New Methods and Properites** |**Description** |
| :- | :- |
|com.aspose.note.INotebookChildNode.getGuid  |Gets the object's globally unique id.  |
|com.aspose.note.Notebook.getGuid  |Gets the object's globally unique id.  |
|com.aspose.note.NotebookLoadOptions.getDeferredLoading  |Gets a value indicating whether children documents should be loaded explicitly later.  |
|com.aspose.note.NotebookLoadOptions.setDeferredLoading(boolean)  |Sets a value indicating whether children documents should be loaded explicitly later.  |
|com.aspose.note.NotebookSaveOptions.getDeferredSaving  |Gets a value indicating whether children documents should be saved explicitly.  |
|com.aspose.note.NotebookSaveOptions.setDeferredSaving(boolean)  |Sets a value indicating whether children documents should be saved explicitly.  |
|com.aspose.note.OneSaveOptions.getDocumentPassword  |Gets a password to encrypt the document content.  |
|com.aspose.note.OneSaveOptions.setDocumentPassword(java.lang.String)  |Sets a password to encrypt the document content.  |
|com.aspose.note.TableCell.getBackgroundColor  |Gets the background color.  |
|com.aspose.note.TableCell.setBackgroundColor(java.awt.Color)  |Sets the background color.  |
|com.aspose.note.Document.save(java.io.OutputStream)  |Saves the OneNote document to a stream.  |
|com.aspose.note.Notebook.#ctor(java.io.InputStream)  |Initializes a new instance of the Notebook class. Opens an existing OneNote notebook from a stream.  |
|com.aspose.note.Notebook.#ctor(java.io.InputStream,com.aspose.note.NotebookLoadOptions)  |Initializes a new instance of the Notebook class. Opens an existing OneNote notebook from a stream. Allows to specify additional loading options.  |
|com.aspose.note.Notebook.loadChildDocument(java.lang.String)  |Adds a child document node. Opens an existing OneNote document from a file.  |
|com.aspose.note.Notebook.loadChildDocument(java.lang.String,com.aspose.note.LoadOptions)  |Adds a child document node. Opens an existing OneNote document from a file. Allows to specify additional load options.  |
|com.aspose.note.Notebook.loadChildDocument(java.io.InputStream)  |Adds a child document node. Opens an existing OneNote document from a stream.  |
|com.aspose.note.Notebook.loadChildDocument(java.io.InputStream,com.aspose.note.LoadOptions)  |Adds a child document node. Opens an existing OneNote document from a stream. Allows to specify additional load options.  |
|com.aspose.note.Notebook.loadChildNotebook(java.lang.String)  |Adds a child notebook node. Opens an existing OneNote notebook from a file.  |
|Acom.aspose.note.Notebook.loadChildNotebook(java.lang.String,com.aspose.note.NotebookLoadOptions)  |Adds a child notebook node. Opens an existing OneNote notebook from a file. Allows to specify additional load options.  |
|com.aspose.note.Notebook.loadChildNotebook(java.io.InputStream)  |Adds a child notebook node. Opens an existing OneNote notebook from a stream.  |
|com.aspose.note.Notebook.loadChildNotebook(java.io.InputStream,com.aspose.note.NotebookLoadOptions)  |Adds a child notebook node. Opens an existing OneNote notebook from a stream. Allows to specify additional load options.  |
|com.aspose.note.Notebook.save(java.io.OutputStream)  |Saves the OneNote document to a stream.  |
|com.aspose.note.Notebook.save(java.io.OutputStream,int/**SaveFormat**/)  |Saves the OneNote document to a stream in the specified format.  |
|com.aspose.note.Notebook.save(java.io.OutputStream,com.aspose.note.NotebookSaveOptions)  |Saves the OneNote document to a file using the specified save options.  |
**Labels:**
