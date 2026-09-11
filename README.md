# -AI-Support-Ticket-Intelligence
End-to-end AI support ticket analysis platform using Hugging Face, semantic search, RAG-style retrieval, Gradio, and SQLite.

## Overview

The platform analyzes a customer support ticket and automatically provides:

- Ticket category classification
- Priority prediction
- Sentiment analysis
- Ticket summarization
- Semantic search for similar historical tickets
- AI-generated suggested responses
- Ticket history stored in SQLite
- Interactive Gradio dashboard

## Example

### Customer Ticket

> I was charged twice for my purchase and want my money back.

### AI Analysis

**Category:** REFUND  
**Priority:** Medium  
**Sentiment:** Negative  

**Summary:**  
Customer was charged twice for their purchase and requests a refund.

The system also retrieves similar refund-related historical tickets and uses them as context to generate a suggested response for a support agent.

## Architecture

```text
Customer Ticket
      ↓
Category Classification
      ↓
Priority Prediction
      ↓
Sentiment Analysis
      ↓
Ticket Summarization
      ↓
Semantic Similarity Search
      ↓
Historical Ticket Retrieval
      ↓
Suggested Response Generation
      ↓
SQLite Database
      ↓
Gradio Dashboard
