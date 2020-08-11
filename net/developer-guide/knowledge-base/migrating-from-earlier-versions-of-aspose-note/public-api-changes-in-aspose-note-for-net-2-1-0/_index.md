---
title: Public API Changes in Aspose.Note for .NET 2.1.0
type: docs
weight: 90
url: /net/public-api-changes-in-aspose-note-for-net-2-1-0/
---

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Note for .NET.
## **Added LoadOptions.DocumentPassword.**
Use LoadOptions.DocumentPassword property to open a password protected document.
## **Added PdfSaveOptions.PageSplittingAlgorithm property and AlwaysSplitObjectsAlgorithm, KeepPartAndCloneSolidObjectToNextPageAlgorithm and KeepSolidObjectsAlgorithm types.**
Use this members to specify page splitting algorithm.
## **Several exception classes were added.**
1. FileCorruptedException - Thrown during document load, when the document appears to be corrupted and impossible to load.
1. IncorrectDocumentStructureException - Thrown if a user created document has incorrect structure.
1. IncorrectPasswordException - Thrown if a document is encrypted with a password and the password specified when opening the document is incorrect or missing.
1. UnsupportedFileFormatException - Thrown during document load, when the file format is not recognized or not supported by Aspose.Note.
1. UnsupportedSaveFormatException - Thrown if requested save format is not supported.
