# Model Context Protocol (MCP) — Theory & Implementation

## Overview

This repository documents my learning and practical implementation of **Model Context Protocol (MCP)**, an open protocol that standardizes how AI applications connect with external tools, resources, and services.

Through this learning journey, I explored MCP architecture, client-server communication, tool calling, resource management, prompt templates, security best practices, and external API integrations using Python.

## Topics Covered

### 1. MCP Fundamentals
- Introduction to Model Context Protocol
- Why MCP is needed
- MCP vs. traditional APIs
- MCP vs. function calling
- Role of MCP in Agentic AI applications

### 2. MCP Architecture
- MCP Host
- MCP Client
- MCP Server
- JSON-RPC communication
- stdio and Streamable HTTP transports
- MCP request lifecycle

### 3. MCP Client
- Connecting to an MCP server
- Discovering available tools
- Calling tools with arguments
- Handling responses and errors

### 4. MCP Server
- Creating an MCP server using Python
- Registering tools and resources
- Defining reusable prompts
- Exposing capabilities to MCP clients

### 5. MCP Tools
- Creating tools with Python decorators
- Tool input schemas and type hints
- Tool execution and validation
- Searching incident records
- Calling external APIs

### 6. MCP Resources
- Understanding MCP resources and URIs
- Reading contextual information
- Resource templates
- Accessing incident reports

### 7. MCP Prompts
- Creating reusable prompt templates
- Passing arguments to prompts
- Retrieving structured investigation instructions

### 8. MCP Security
- Input validation
- Authentication and authorization concepts
- Principle of least privilege
- Secure handling of credentials
- Prompt injection risks
- Human approval for sensitive operations

### 9. Connecting Agents to External Systems
- Integrating REST APIs with MCP tools
- Connecting AI applications to external services
- Understanding MCP with agent frameworks
- MCP and RAG integration concepts

## Practical Implementation

The implementations are designed for **Google Colab** using Python and the MCP Python SDK.

The practical exercises include:

- A mathematical MCP server with addition and multiplication tools.
- An incident-search tool for retrieving relevant incident records.
- An incident-report resource using URI templates.
- Reusable prompts for incident investigation.
- An external REST API integration using JSONPlaceholder.
- An integrated workflow combining incident search, resource reading, and prompt retrieval.
- Basic input validation and security exercises.

## Mini Project: Incident Investigation MCP Server

The mini project demonstrates how MCP capabilities can be combined to support a production incident investigation workflow.

**Key components:**
- **Tools:** Search incident records and retrieve external data.
- **Resources:** Access structured incident reports.
- **Prompts:** Generate investigation instructions.
- **Client:** Discover and invoke server capabilities.

The implementation demonstrates retrieval and preparation of investigation context. It can be extended with an LLM, LangGraph, log analysis, and evidence-based root-cause investigation.

## Tech Stack

- Python
- Model Context Protocol (MCP)
- MCP Python SDK
- Google Colab
- REST APIs
- JSON / JSON-RPC
- Async Python

## Learning Outcomes

Through this implementation, I learned how to:

- Understand MCP's client-server architecture.
- Create and register MCP tools, resources, and prompts.
- Connect MCP clients to server capabilities.
- Integrate external REST APIs through MCP tools.
- Apply input validation and least-privilege principles.
- Understand how MCP supports AI agents and external system integrations.

## Future Improvements

- Connect an LLM to MCP tools.
- Integrate MCP with LangChain or LangGraph.
- Add database and document-retrieval tools.
- Implement authenticated remote MCP access.
- Build an evidence-based AI incident investigation agent.
- Add automated tests and evaluation.

## References

- [Official MCP Documentation](https://modelcontextprotocol.io/)
- [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk)
- [Python SDK Documentation](https://py.sdk.modelcontextprotocol.io/)

---

**Learning Focus:** Generative AI | Agentic AI | Model Context Protocol | AI Engineering
