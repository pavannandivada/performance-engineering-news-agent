# Performance Engineering News Agent

## Overview

The Performance Engineering News Agent is an AI-powered automation project designed to discover relevant performance engineering and observability content, evaluate its relevance, generate original insights, and eventually publish selected content to LinkedIn.

The project is being built incrementally using n8n, AI models, GitHub, and performance engineering concepts.

## Goal

The long-term goal is to create an automated system that can:

1. Monitor trusted performance engineering and technology sources.
2. Identify newly published content.
3. Filter duplicate and irrelevant content.
4. Evaluate whether an article is useful to performance engineers.
5. Extract the important technical insight.
6. Generate an original LinkedIn post based on the insight.
7. Publish the post automatically.
8. Maintain a record of processed content to avoid duplicates.

## High-Level Architecture

```text
Trusted Sources
      |
      v
   n8n Scheduler
      |
      v
 Content Collection
      |
      v
Duplicate Detection
      |
      v
   AI Analysis
      |
      v
Relevance Scoring
      |
      v
Technical Insight
      |
      v
LinkedIn Post Generation
      |
      v
LinkedIn Publishing
      |
      v
Processing History
Technology Stack
n8n - Workflow automation
Google Gemini - AI analysis and content generation
GitHub - Source control and project documentation
LinkedIn - Content publishing
RSS / APIs - Content ingestion
Docker - Local n8n environment
Development Approach
The project will be developed incrementally.
Each significant improvement will be implemented as a GitHub pull request so that the repository documents the evolution of the system.
Planned milestones include:
Initial project architecture
Trusted content source integration
Content filtering
Duplicate detection
AI relevance scoring
Technical insight extraction
LinkedIn content generation
Automated LinkedIn publishing
Scheduling and persistence
Monitoring and error handling
Security
Credentials and API keys must never be committed to the repository.
Secrets should be stored using the appropriate credential management mechanisms provided by the automation platform or environment.
Current Status
The initial n8n environment has been deployed locally using Docker.
A basic workflow has been created to pass an idea to an LLM and generate a LinkedIn post.
This workflow is currently a proof of concept and will evolve into the automated Performance Engineering News Agent.
