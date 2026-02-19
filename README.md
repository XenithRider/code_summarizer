

# Code Summarizer 
This application is a Gradio-based tool designed to automatically analyze and summarize code files (JavaScript, TypeScript, Python, etc.) using Large Language Models (LLMs). It transforms complex source code into human-readable documentation, which can be viewed in the browser or downloaded as a professional DOCX report.

## Features
**Multi-File Support:** Upload multiple code files at once for batch processing.

**AI-Powered Analysis:** Leverages Meta-Llama-3.1-70B via Together.ai to identify key functions, classes, and dependencies.

**Structured Summaries:** Generates clear, bulleted explanations of code purpose, inputs, and outputs.

**Professional Reporting:** Automatically formats summaries into a DOCX document with proper headings and organization.

**Interactive UI:** Simple, web-based interface built with Gradio for easy file handling.

## Architecture
### The system follows a three-stage processing pipeline:

**Input Interface:** Users upload files via the Gradio UI.

**Processing Pipeline:** Files are read, and their content is sent to the Together.ai API for summarization.

**Output Generation:** Summaries are formatted into a DOCX file using python-docx and presented to the user for download.
