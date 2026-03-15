# cymbal-universal-employee-portal-docs
Docs for the project that builds a universal employee portal using Vertex AI Search to answer HR and internal financial questions.

## Introduction
Imagine that you work at Cymbal, a massive, global online shopping business. Employees such as you have many internal questions daily: "What is our policy for booking business travel?", or "How many units of sneakers did we sell last month?"

Typically, you must sign in to completely different systems to find these answers. In addition to dealing with different systems, you must also read through a large number of unstructured HR data or run complex SQL prompts on structured financial data to get answers to your questions.

This codelab helps you build a single, unified internal app for all employees. You then connect the app to employee HR documents and internal financial records. This architecture also lets you add IT, marketing, and sales data later to make the app even more comprehensive.

## Product architecture
To build this quickly without managing complex machine learning infrastructure, use these Google Cloud tools:

* Vertex AI Search: Vertex AI Search is the core of your application. It is a fully-managed AI search engine that understands the semantic meaning of a question. It functions as an out-of-the-box Retrieval Augmented Generation (RAG) system. This means it can simultaneously read unstructured data, for example, PDFs, and structured data, for example, databases, to return a conversational, AI-generated summary of the answer.
  
* Cloud Storage: Cloud Storage is a highly-scalable cloud hard drive. In this codelab, you use a public Cloud Storage bucket that contains real-world mock PDFs for Cymbal employees, such as travel policies, benefits, and handbooks.
  
* BigQuery: BigQuery is Google's enterprise data warehouse. In this codelab, you use a public BigQuery dataset that contains thousands of mock internal financial trade records for Cymbal, organized in rows and columns.
Note: The codelab does not cover how to host this app on Cloud Run. 

