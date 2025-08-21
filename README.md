# RAG-Based-AI-Social-Media-Marketing-Campaign-Assistant
An AI Social Media Marketing Campaign Assistant that uses RAG to integrate Iconic Ad Campaigns

## Table of Contents

- [Overview](#overview)
- [Situation](#situation)
- [Task](#task)
- [Action](#action)
- [Result](#results)    
- [Technologies Used](#technologies-used)
- [Demo](#demo)  

## Overview

The AI Social Media Marketing Campaign Assistant leverages RAG to enhance marketing strategy development by combining pre-existing campaign knowledge with dynamic AI generation. By integrating a vector-based retrieval system with GPT-4o, the system can pull insights from a database of iconic ad campaigns and provide creative recommendations, content suggestions, and marketing strategies tailored to current social media trends.

## Situation

Marketing teams often face challenges such as:
1. Generating fresh, campaign-specific ideas while maintaining brand alignment.
2. Accessing historical successful campaigns for inspiration.
3. Efficiently analyzing large volumes of campaign data to extract relevant insights.

Traditional approaches are time-consuming and may overlook subtle connections between campaigns. The RAG-based AI assistant addresses these challenges by combining structured campaign knowledge with generative AI to provide real-time, contextually grounded recommendations.

## Task 

1. Build an AI assistant that can retrieve and summarize relevant campaign data based on user queries.
2. Implement a system that guides social media marketing decisions using both historical campaign insights and AI-generated suggestions.
3. Ensure scalable, cloud-based deployment that integrates seamlessly with Azure AI services.

## Action

1. Deploy the GPT-4o model and the Embedding Model
  a.Use GPT-4o for chat and generative capabilities.
  b.Use text-embedding-ada-002 for vectorizing campaign content.
2. Create Vector Index for Uploaded Campaign Data
  a.Chunk and embed campaign data.
  b.Create an Azure AI Search index to store embeddings.
  c.Register the index as a searchable asset.
3. Test the Index in the Playground
  a.Query the index with sample prompts to validate retrieval quality.
4. Implement RAG Pattern Using Azure OpenAI SDK
  a.Instantiate an Azure OpenAI client using endpoint and credentials.
  b.Set up a system message to contextualize responses (e.g., “You are an AI assistant that integrates iconic ad campaigns into social media strategies.”)
  c.Submit user prompts with:
    i. Index connection details for relevant campaign retrieval.
    ii. Embedding model specification for vectorization.
5. Receive and display grounded responses.
6. Append responses to the chat history for context-aware follow-ups.

## Result

Reduced time-to-insight by integrating historical campaigns with AI-generated recommendations.

## Technologies Used

1. Language Model: GPT-4o
2. Embedding Model: text-embedding-ada-002 
3. Cloud AI Platform: Azure AI Foundry
4. Python SDKs:
    a. azure-ai
    b. python-dotenv (environment variable management)
5. Development Environment: Azure Cloud Shell / Local Python
6. Version Control & Hosting: Git & GitHub

##References

https://www.adsoftheworld.com/campaigns/

## Demo

![RAG-Based-AI-Social-Media-Marketing-Campaign-Assistant-Demo-GIF](https://github.com/user-attachments/assets/7b3d606d-de5b-48b2-91a7-10746e303cce)

FULL VIDEO DEMO LINK: 

LINK: https://drive.google.com/drive/folders/1XQYrQqkeJJGe9foyTDGOCrLVDVlcu2zU?usp=sharing
