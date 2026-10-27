# Multi-Agent E-commerce RAG

A multi-agent e-commerce support system built with Amazon Bedrock, demonstrating orchestrated agent collaboration, retrieval-augmented generation, shared state, and customer response coordination.

## Overview

This project demonstrates a multi-agent architecture for handling e-commerce support workflows. Instead of relying on a single agent, the system uses an orchestrator agent to coordinate multiple specialist agents responsible for different tasks such as inventory support, policy retrieval, refund reasoning, and customer communication.

The project also incorporates retrieval-augmented generation (RAG) to ground policy-related responses in reference material, helping improve response relevance and reliability.

## Architecture and Workflow

![Project Architecture](images/architecture-project-3.png)


The architecture follows a multi-agent orchestration workflow:

- **User**: The workflow begins when a customer submits an e-commerce-related request.
- **Orchestrator Agent**: A central orchestrator receives the request and delegates work to the appropriate specialist agents.
- **Inventory Agent**: Handles product availability and inventory-related questions.
- **Policy Agent**: Handles store policy questions and uses retrieval to ground responses in reference material.
- **Refund Agent**: Handles refund-related reasoning and decision support.
- **Communication Agent**: Helps prepare clear customer-facing responses based on the outputs of the specialist agents.
- **Knowledge Base Retrieval**: Supports the Policy Agent by retrieving relevant policy information from the knowledge base.
- **Shared State / Observability**: Maintains coordination context across agents and supports monitoring of the overall workflow.
- **Final Customer Response**: The orchestrated result is returned to the customer as a final response.

## My Contributions

In this project, I:
- Built the orchestration workflow for coordinating specialist agents
- Designed routing across inventory, policy, refund, and communication tasks
- Incorporated retrieval-based grounding for policy-related responses
- Supported shared context across the multi-agent workflow
- Tested system behavior through logs and workflow inspection
- Documented architecture decisions and possible improvements

## Key Findings

This project strengthened my understanding of multi-agent system design, orchestration patterns, retrieval-augmented generation, and shared-state coordination. It also provided practical experience in building AI systems that combine specialized agent roles into a unified customer support workflow.
