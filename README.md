# Intelligent Document Processing (IDP) Using Databricks

An exploratory project demonstrating how **Intelligent Document Processing (IDP)** can transform unstructured PDF documents into structured, usable data using Databricks and AI-assisted document processing.

## Project Overview

Documents such as invoices, purchase orders, and receipts often contain valuable information in unstructured formats. Extracting this information manually can be time-consuming and difficult to scale.

This project explores an AI-powered document processing workflow in Databricks to ingest PDF files, parse their contents, identify document types, and extract relevant information into structured datasets.

The goal is to make information from unstructured documents easier to process, organize, and use for downstream analytics.

## Technologies Used

- **Databricks** – Data processing and analytics environment
- **Python / SQL** – Data processing and transformation
- **AI Parse Document (`ai_parse_document`)** – Parsing document content
- **AI Classification (`ai_classify`)** – Identifying and categorizing document types
- **Delta Lake** – Structured data storage within the Databricks environment

## Project Workflow

The project follows an end-to-end document processing workflow:

1. **Document Ingestion**
   - Upload PDF documents, such as invoices, purchase orders, and receipts, into a Databricks Volume.
   - Access document files and metadata using Databricks SQL.

2. **Document Parsing**
   - Read PDF files using the `read_files` function.
   - Process document content using `ai_parse_document`.
   - Extract available text, tables, and other document elements.

3. **Intermediate Data Storage**
   - Store parsed document content and file paths in an intermediate table.
   - Transform parsed document elements into readable text for further processing.

4. **Document Classification**
   - Use AI-assisted classification to identify document categories.
   - Separate invoices, purchase orders, and receipts based on their content.

5. **Information Extraction**
   - Identify and extract relevant fields from each document type.
   - Examples include invoice IDs, total amounts, and other relevant document information.

6. **Structured Data Transformation**
   - Organize extracted information into structured datasets.
   - Prepare the resulting data for downstream reporting and analysis.

## Key Concepts Explored

- Intelligent Document Processing (IDP)
- Processing unstructured PDF documents
- Document ingestion and content parsing
- AI-assisted document classification
- Information and field extraction
- SQL-based data transformation
- Structured data preparation for analytics
- Databricks data storage and processing

## Example Use Cases

The workflow demonstrates how different document types can be processed into structured information:

| Document Type | Example Information |
|---|---|
| Invoice | Invoice ID, total amount, and other invoice details |
| Purchase Order | Purchase order information and relevant fields |
| Receipt | Receipt details and transaction information |

## Learning Outcomes

Through this project, I explored how Databricks AI capabilities can simplify the processing of unstructured documents and convert their contents into structured, analytics-ready data.

The project provided practical exposure to document ingestion, AI-assisted parsing and classification, content extraction, and structured data transformation.



---

**Project:** Intelligent Document Processing (IDP) Using Databricks  
**Domain:** Data Engineering | AI/ML | Document Processing  
**Tools:** Databricks, Python, SQL, AI Parse Document, AI Classification, Delta Lake
