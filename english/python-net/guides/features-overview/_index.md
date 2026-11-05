---
title: Features Overview
linkTitle: "Features overview"
second_title: GroupDocs.Parser for Python via .NET API References
description: "GroupDocs.Parser for Python via .NET extracts text, formatted text, tables, images, hyperlinks, metadata and annotations through a single, format-independent API, and parses documents by templates."
type: docs
url: /python-net/guides/features-overview/
is_root: false
weight: 50
---


GroupDocs.Parser for Python via .NET extracts data from a wide range of [supported document formats](https://docs.groupdocs.com/parser/python-net/supported-document-formats/). Every operation follows the same workflow: open a document with [`Parser`](/parser/python-net/groupdocs.parser/parser/), call an extraction method such as `get_text()`, `get_tables()` or `get_metadata()`, and read the result. A method returns `None` when the document's format does not support that operation, so one code path serves every format.

## Text extraction

Extract the plain text of a whole document or of one page. The accurate mode keeps the reading order and layout; the raw mode is faster and fits pipelines where speed matters more than layout. Scanned pages and images are read with OCR. See [Extract text from documents](/parser/python-net/guides/extract-text-from-documents/), [Extract text in Accurate mode](https://docs.groupdocs.com/parser/python-net/extract-text-in-accurate-mode/), and [Extract text in Raw mode](https://docs.groupdocs.com/parser/python-net/extract-text-in-raw-mode/).

## Formatted text

`get_formatted_text()` returns HTML, Markdown or plain text that keeps the document's headings, numbered and bulleted lists, tables, hyperlinks, and bold and italic text, ready for an HTML preview or a Markdown pipeline. See [Working with Text](https://docs.groupdocs.com/parser/python-net/working-with-text/).

## Search, structure, and text areas

Search a document by keyword or regular expression and get the text around each hit, read its structure (paragraphs, headings, lists, tables and hyperlinks) as XML, or get its text areas with their coordinates and text style. See [Search text](/parser/python-net/guides/search-text/), [Extract highlights](https://docs.groupdocs.com/parser/python-net/extract-highlights/), [Extract text structure](https://docs.groupdocs.com/parser/python-net/extract-text-structure/), and [Extract text areas](https://docs.groupdocs.com/parser/python-net/extract-text-areas/).

## Tables

Extract the tables of PDF, Word, spreadsheet and presentation pages with their rows and cells, from a whole document or one page. See [Extract tables from document](/parser/python-net/guides/extract-tables-from-document/) and [Extract tables from document page](https://docs.groupdocs.com/parser/python-net/extract-tables-from-document-page/).

## Images and hyperlinks

Extract the images of a document, a page or a rectangular page area, and save them to files in their own format or another. Hyperlinks are extracted the same way. See [Extract Images from Documents](/parser/python-net/guides/extract-images-from-documents/), [Extract images to files](https://docs.groupdocs.com/parser/python-net/extract-images-to-files/), and [Extract hyperlinks from document](/parser/python-net/guides/extract-hyperlinks-from-document/).

## Metadata and document information

Read document properties such as title, author and dates with `get_metadata()`, the table of contents with `get_toc()`, and the file type, page count and size with `get_document_info()`. List every format the library reads with `FileType.get_supported_file_types()`. See [Extract Metadata from Documents](/parser/python-net/guides/extract-metadata-from-documents-2/), [Get document info](/parser/python-net/guides/get-document-info/), and [Get supported file formats](/parser/python-net/guides/get-supported-file-formats/).

## Annotations

Read the comments and notes reviewers leave in PDF, Word and PowerPoint files. Call `get_annotations()` for the whole document, or `get_annotations(page_index)` for one page; each annotation carries its text, type, page, author and timestamp. To get the annotations' text inside the extracted text, set `TextOptions.include_annotations`. See [Working with annotations](https://docs.groupdocs.com/parser/python-net/working-with-annotations/).

## Templates

Describe the fields and tables of documents that share a layout, such as invoices, once in a template, then pass it to `parse_by_template()` to read their values from every such document. See [Parse Data from Documents](/parser/python-net/guides/parse-data-from-documents/) and [Working with Templates](/parser/python-net/guides/working-with-templates/).

## Archives, attachments, and portfolios

`get_container()` lists the documents inside ZIP, RAR, 7Z and TAR archives, email attachments, Outlook data files and PDF portfolios, and each item opens with a [`Parser`](/parser/python-net/groupdocs.parser/parser/) of its own. See [Extract Data from Attachments and ZIP Archives](/parser/python-net/guides/extract-data-from-attachments-and-zip-archives/) and [Working with Containers](https://docs.groupdocs.com/parser/python-net/working-with-containers/).

## Loading documents

Open a document from a file path or a binary stream, open password-protected documents, and tell the library a document's format when its name does not. See [Load file from stream](https://docs.groupdocs.com/parser/python-net/load-file-from-stream/) and [Load password-protected documents](/parser/python-net/guides/load-password-protected-documents/).

## Logging and external resources

Pass a Python function, or an object with `trace`, `warning` and `error` methods, to [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings/) to receive the engine's log messages. A resource handler decides which images an HTML or MHTML document may load. See [Logging](https://docs.groupdocs.com/parser/python-net/logging/) and [Handle loading of external resources](https://docs.groupdocs.com/parser/python-net/handle-loading-of-external-resources/).

## Command line

The package installs the `groupdocs-parser` command, which extracts text, document info, metadata, images and annotations without writing Python code. See [Command Line Interface](/parser/python-net/guides/command-line-interface/).

## On-premise

GroupDocs.Parser for Python via .NET runs entirely on your own infrastructure — your documents never leave your environment. The package is a self-contained wheel that bundles everything it needs, so no Microsoft Office, OpenOffice, or separate runtime has to be installed. See [System Requirements](https://docs.groupdocs.com/parser/python-net/system-requirements/) for the supported platforms and native dependencies.
