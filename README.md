# Rowdy-Rez
Rowdy Rez! 🤙your go-to guide for UTSA campus resources. No more searching, just ask!

# Rowdy Rez — AI-Powered Student Resource Copilot

An AI-powered assistant built to solve a critical student problem: discovering campus resources when they need them most.

• Researched 245+ students to identify resource awareness as the #1 pain point  
• Designed and deployed a conversational AI agent inside Microsoft Teams  
• Enabled instant, contextual answers for campus resources (location, hours, contact)  
• Piloted with graduate assistants and student outreach initiatives  

Built using Microsoft Copilot Studio + Azure OpenAI (RAG-based architecture)

## The Problem

At the University of Texas at San Antonio (UTSA), students have access to dozens of support services — tutoring, mental health, food assistance, and career services.

However, a structured research study revealed a critical gap:

• Surveyed 245 students across undergraduate, graduate, and doctoral programs  
• #1 pain point: Students did not know what resources existed  
• Repeated sentiment: “I wish I had known about this earlier”  

### Key Insight
The problem was not access — it was discoverability.

Existing solutions (websites, portals, chatbots) required:
- Manual searching  
- Prior awareness  
- Navigation across multiple pages  

Students needed a **faster, more intuitive way to find help**.

## Solution — Rowdy Rez

I designed Rowdy Rez, a conversational AI assistant that allows students to ask questions in natural language and instantly receive relevant campus resource information.

### Design Principles

• Zero friction — no new apps or logins  
• Meet students where they are — Microsoft Teams  
• Natural language interaction — “ask like a friend”  
• High accuracy — grounded in verified university data  
• Scalable — supports thousands of students without additional staff  

## System Design

Rowdy Rez uses a Retrieval-Augmented Generation (RAG) approach to ensure accurate, context-aware responses.

### How It Works

1. User asks a question in Microsoft Teams  
2. The system retrieves relevant information from curated UTSA resource sources  
3. The AI generates a response grounded in that data  

### Why RAG?

Traditional chatbots:
- Rely on predefined rules or FAQs  
- Can provide generic or incomplete answers  

RAG-based systems:
- Retrieve real data before generating responses  
- Reduce hallucination risk  
- Provide specific, actionable answers (location, hours, contact info)  

### Implementation Approach

Built using Microsoft Copilot Studio’s agent framework with:
- Restricted knowledge sources (only verified UTSA resources)  
- Structured knowledge inputs (location, hours, contact fields)  
- Instruction-based response formatting

## What I Built

While leveraging Microsoft Copilot Studio’s infrastructure, I was responsible for designing and configuring the agent’s intelligence and behavior.

### Key Contributions

• Defined strict instruction set to:
  - Limit responses to UTSA resources only  
  - Reject unrelated queries (e.g., math, coding, general knowledge)  

• Engineered response structure:
  - Always prioritize location, hours, and contact info  
  - Ensure consistency across responses  

• Curated knowledge base:
  - Aggregated 30+ verified resource links  
  - Structured information for retrieval accuracy  

• Designed conversation experience:
  - Created suggested prompts for common student needs  
  - Optimized for first-time usability  

• Conducted iterative testing:
  - Tested across multiple real-world student scenarios  
  - Refined prompts and constraints based on behavior

## Validation & Early Signals

Rowdy Rez was piloted through:

• Graduate assistant usage  
• Student outreach during tabling events  
• Live demonstrations to students  

### Observations

• Students quickly understood how to use the system  
• Reduced need to navigate multiple websites  
• Positive engagement during live interactions  

### Key Learning

Even in early-stage testing, students showed strong preference for:
→ Asking questions conversationally instead of searching manually  

(This project is currently in early validation stage; formal usage analytics and A/B testing are planned next.)

## Trade-offs & Limitations

• Limited knowledge sources (free-tier constraints)  
• Inconsistent retrieval for deeply specific queries  
• Partial reliance on prompt constraints for guardrails  
• No analytics tracking implemented yet  

### Key Trade-off

Speed of deployment vs. system robustness  
→ Chose rapid prototyping to validate user need before full-scale build  

## Future Improvements

• Implement analytics to track usage and accuracy  
• Expand knowledge base using structured documents  
• Improve retrieval consistency for edge cases  
• Integrate with university platforms (Canvas, myUTSA)  
• Launch pilot with measurable success metrics  

## Key Learnings

• Discoverability is often a bigger problem than access  
• Semantic search significantly improves user experience over keyword search  
• Prompt engineering is critical for controlling AI system behavior  
• Low-code AI tools can accelerate product development when paired with strong problem definition  
• Early-stage validation should prioritize user behavior over perfect metrics  
