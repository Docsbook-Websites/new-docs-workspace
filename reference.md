```yaml
title: "DocuSphere Command Reference for Document Management"
description: "Access DocuSphere commands for document creation and collaboration. Streamline your workflow with this comprehensive reference guide."
---

# DocuSphere Command Reference

This reference guide provides a comprehensive overview of commands available in DocuSphere for document management. Use these commands to enhance your document creation and collaboration experience.

## Document Creation Commands

| Parameter/Command     | Type         | Description                                         | Example                        |
|-----------------------|--------------|-----------------------------------------------------|--------------------------------|
| `createDocument`      | Function     | Initiates a new document in the workspace.         | `createDocument("Project Plan")` |
| `setTitle`            | Function     | Sets the title of the current document.            | `setTitle("Meeting Notes")`   |
| `addText`             | Function     | Inserts text into the document at the current cursor position. | `addText("This is a new section.")` |
| `insertImage`         | Function     | Adds an image to the document from your device.    | `insertImage("/path/to/image.png")` |

## Collaboration Commands

| Parameter/Command     | Type         | Description                                         | Example                        |
|-----------------------|--------------|-----------------------------------------------------|--------------------------------|
| `shareDocument`       | Function     | Shares the document with specified users.          | `shareDocument(["user1@example.com", "user2@example.com"])` |
| `comment`             | Function     | Adds a comment to the document for collaboration.   | `comment("Please review this section.")` |
| `trackChanges`        | Function     | Enables change tracking for the document.          | `trackChanges(true)`          |
| `resolveComment`      | Function     | Marks a comment as resolved.                        | `resolveComment("comment_id")` |

## Formatting Commands

| Parameter/Command     | Type         | Description                                         | Example                        |
|-----------------------|--------------|-----------------------------------------------------|--------------------------------|
| `boldText`            | Function     | Applies bold formatting to selected text.          | `boldText("Important")`       |
| `italicizeText`       | Function     | Applies italic formatting to selected text.        | `italicizeText("Note")`       |
| `createList`          | Function     | Creates a bulleted or numbered list.               | `createList(["Item 1", "Item 2"])` |
| `insertTable`         | Function     | Inserts a table into the document.                 | `insertTable(3, 2)`           |

## Document Management Commands

| Parameter/Command     | Type         | Description                                         | Example                        |
|-----------------------|--------------|-----------------------------------------------------|--------------------------------|
| `saveDocument`        | Function     | Saves the current document.                         | `saveDocument()`              |
| `deleteDocument`      | Function     | Deletes the specified document from the workspace. | `deleteDocument("doc_id")`    |
| `exportDocument`      | Function     | Exports the document in various formats.           | `exportDocument("PDF")`       |
| `importDocument`      | Function     | Imports a document from an external source.        | `importDocument("/path/to/file.docx")` |

Use this reference to navigate the powerful features of DocuSphere and enhance your document management workflow.
```