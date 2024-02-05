# Indexify

Indexify is a reactive compute engine for extracting unstructured data and building Indexes. If you are building RAG LLM Applications or Agents which depend on data that are in unstructured documents or video/audio, Indexify can help you to build pipelines which keeps your indexes updated in real time as data changes.

## Modules 
### Indexify Server
Indexify Server is the control plane which sits on top of databases like vector stores, structured stores and blob stores to ingest unstructured data and write to Indexes. 

### Extractors
Extractors are Python classes which extracts embedding or JSON metadata from unstructured data sources. We have built some common extractors for extracting embedding, information from PDF documents, video and audio here - http://github.com/tensorlakeai/indexify-extractors

### Extractor SDK
If you would like to build a new extractor for your specific usecase, you can use the Extractor SDK here which has the tools to build, test and package extractors that can be used with Indexify. The SDK is available on PyPI and the code lives here - https://github.com/tensorlakeai/indexify_extractor_sdk

### Indexify Client API 
Python API to interact with the Indexify server API to upload content and retreive and search indexes is available as a package on PyPI and the code lives here - https://github.com/tensorlakeai/indexify/tree/main/sdk-py 
