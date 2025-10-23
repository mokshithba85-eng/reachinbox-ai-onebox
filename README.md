# reachinbox-ai-onebox

# ReachInbox Onebox - Email Aggregator System

> 🚀 AI-Powered Email Management Platform with Real-time Multi-Account Synchronization

[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch)](https://www.elastic.co/)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)

## 📝 Overview

A sophisticated email aggregator system built for ReachInbox that synchronizes multiple IMAP email accounts in real-time, provides AI-powered email categorization, intelligent search capabilities, and automated notifications. This system demonstrates advanced full-stack development with modern technologies and AI integration.

## ✨ Features Implemented

### 🔄 Feature 1: Real-Time Email Synchronization
- ✅ **Multi-Account Support**: Synchronizes 2+ IMAP accounts simultaneously
- ✅ **Historical Data**: Fetches last 30 days of emails from each account
- ✅ **Real-Time Updates**: Uses IMAP IDLE mode for instant email notifications (no polling)
- ✅ **Connection Management**: Persistent connections with automatic reconnection handling
- ✅ **Email Parsing**: Complete extraction of headers, body, attachments, and metadata

### 🔍 Feature 2: Searchable Storage with Elasticsearch
- ✅ **Docker Integration**: Local Elasticsearch instance via Docker Compose
- ✅ **Advanced Indexing**: Optimized email indexing for lightning-fast searches
- ✅ **Multi-Filter Support**: Filter by account, folder, date range, and category
- ✅ **Full-Text Search**: Search across email subject, body, and sender information
- ✅ **Pagination**: Efficient handling of large email datasets

### 🤖 Feature 3: AI-Based Email Categorization
- ✅ **5-Label Classification**: Automatically categorizes emails into:
  - **💚 Interested** - Shows engagement with offers/products
  - **💙 Meeting Booked** - Meeting confirmations and scheduling
  - **❤️ Not Interested** - Declines or shows no interest
  - **🖤 Spam** - Promotional, irrelevant, or suspicious content
  - **💛 Out of Office** - Auto-reply and unavailability messages
- ✅ **AI Integration**: OpenAI GPT-4 / Google Gemini API integration
- ✅ **High Accuracy**: Fine-tuned prompts for precise categorization

### 📢 Feature 4: Slack & Webhook Integration
- ✅ **Slack Notifications**: Instant notifications for "Interested" category emails
- ✅ **Webhook Automation**: Triggers webhook.site for external integrations
- ✅ **Rich Messaging**: Detailed email information in notifications
- ✅ **Error Handling**: Robust notification delivery with retry mechanisms

### 💻 Feature 5: Frontend Interface
- ✅ **Modern React UI**: Clean, responsive email client interface
- ✅ **Multi-Account Display**: Unified inbox view for all connected accounts
- ✅ **Advanced Filtering**: Filter by account, folder, category, and date
- ✅ **Real-Time Search**: Elasticsearch-powered instant search
- ✅ **Category Visualization**: Color-coded AI category badges
- ✅ **Mobile Responsive**: Optimized for all screen sizes

### 🧠 Feature 6: AI-Powered Suggested Replies (RAG)
- ✅ **Vector Database**: Pinecone integration for context storage
- ✅ **RAG Implementation**: Retrieval-Augmented Generation for intelligent replies
- ✅ **Context-Aware**: Personalized responses based on stored training data
- ✅ **Job Application Context**: Specialized for job-seeking scenarios
- ✅ **Smart Suggestions**: AI-generated contextual email responses


## 🛠️ Tech Stack

### Backend Technologies
- **Runtime**: Node.js 18+ with TypeScript
- **Framework**: Express.js for REST API
- **Email Processing**: `imap` library with `mailparser`
- **Search Engine**: Elasticsearch 8.11
- **AI Services**: OpenAI GPT-4 API / Google Gemini
- **Vector Database**: Pinecone (for RAG functionality)
- **Notifications**: Slack Webhook API

### Frontend Technologies
- **Framework**: React 18 with TypeScript
- **Styling**: Tailwind CSS
- **State Management**: React Context API + Hooks
- **HTTP Client**: Axios
- **Routing**: React Router v6

### Infrastructure & DevOps
- **Containerization**: Docker & Docker Compose
- **Development**: Nodemon, ts-node
- **Code Quality**: ESLint, Prettier
- **Version Control**: Git with conventional commits

## 🚀 Quick Start Guide

### Prerequisites
- Node.js 18 or higher
- Docker and Docker Compose
- Git
- Code editor (VSCode recommended)
- 
Commands to execute in command prompt 
 # 1️ ⃣ Navigate to your project folder
cd C:\Users\Mokshith B A\reachinbox-onebox
# 2️ ⃣ Start Docker containers (Elasticsearch & Qdrant)
docker-compose up -d
# 3️ ⃣ Verify containers are running
docker ps
# 4️ ⃣ Install dependencies
npm install
# 5️ ⃣ Run the backend server
npm run dev
# 6️ ⃣ Open the frontend (index.html) in your browser
start index.html




