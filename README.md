# Internal Knowledge Assistant with Role-Based Access Control

## Overview

Designed and implemented a Retrieval-Augmented Generation (RAG) based internal chatbot that enables secure, role-specific access to organizational knowledge.  
The system enforces fine-grained access control, ensuring users retrieve only the information permitted for their assigned department.

---

## Problem Statement

Organizations require internal AI assistants that provide accurate knowledge retrieval while maintaining strict data boundaries across departments.  
This project simulates an enterprise-grade internal chatbot capable of context-aware response generation with enforced role-based access policies.

---

## Key Features

### Role-Based Access Control (RBAC)
Access restrictions implemented across departments:
- Engineering  
- Finance  
- HR  
- Marketing  
- General  

### Secure Authentication
- HTTP Basic Authentication using FastAPI  
- User-role validation before query execution  

### Retrieval-Augmented Generation Pipeline
- Document ingestion and preprocessing  
- Text chunking and embedding generation  
- Vector indexing for semantic similarity search  
- Context-aware response synthesis using LLMs  

### Scalable Architecture
- Modular pipeline design  
- Separation of authentication, retrieval, and generation layers  
- Easily extendable to additional departments or data sources  

---

## Tech Stack

- Python  
- FastAPI  
- LangChain  
- Vector Database (Qdrant)  
- LLM + Embeddings  
- Role-based filtering middleware  

---

## System Workflow

1. User authentication via HTTP Basic Auth  
2. Role validation and access control enforcement  
3. Query embedding generation  
4. Role-filtered vector similarity search  
5. Context retrieval  
6. LLM-based response generation  

---

## Outcome

Developed a secure internal AI assistant that demonstrates:
- Controlled information access
- Semantic search capabilities
- Production-style backend architecture
- Enterprise-aligned security considerations
