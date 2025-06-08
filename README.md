# Meta-Data-Extraction

About the Project
This project automates the extraction of metadata from lease agreement documents in PDF format. Lease documents often contain complex legal language, clauses, and structured data buried within unstructured text. This tool processes those documents and extracts meaningful insights using modern NLP techniques.

🔍 What is Metadata in this Context?
In the context of lease documents, metadata refers to summarized and structured information automatically derived from the full text. This includes:

Document Summary – A concise overview of the lease content

Key Topics – Main themes or clauses discussed (e.g., liability, payment terms)

Keywords – Important terms/phrases like “lessor,” “termination,” “payment schedule”

Named Entities – Recognizable names of people, organizations, dates, monetary values, locations, etc.

Sentiment Analysis – General tone of the text (e.g., neutral, negative)

Readability Score – How easy or difficult the text is to read (Flesch Reading Ease)

Relevant Sentences – Contextually similar sentences to a user-defined query (e.g., “lease agreement”)

These outputs help legal analysts, real estate managers, or software systems quickly understand the key components of a lease without manually reading through dozens of pages.

Example Use Case
A user uploads a lease PDF. The system processes the document, and in return, they receive:

A summary of the lease terms

Identified parties (e.g., names of lessee, lessor)

Important dates and monetary amounts

Key clauses or obligations

A list of recurring legal keywords

Sentiment trend of the agreement

Readability score (helpful for layman comprehension)

Ideal Input Documents
Lease or rental agreements (in PDF format).....

This project extracts metadata from lease agreement PDFs using a combination of NLP tools. It performs summarization, keyword extraction, topic modeling, named entity recognition, sentiment analysis, and more from unstructured lease document content.

📥 Input
PDF documents containing lease agreements (e.g., HLRBO_Template_Lease_Document.pdf)

Uploaded via a path (default: /content/HLRBO_Template_Lease_Document.pdf in Colab)

📤 Output
For each lease document, the script extracts:

📚 Summary (using T5 transformer)

🧠 Topics (using Gensim LDA)

🔑 Keywords (using KeyBERT)

🏷️ Named Entities (using spaCy)

📈 Sentiment (using Hugging Face sentiment analysis pipeline)

📊 Readability Score (Flesch Reading Ease)

🔍 Most Relevant Sentences for a specific query (e.g., "lease agreement")

Contracts or property terms

Any legal document structured similarly to leases
