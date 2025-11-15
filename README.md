# Agents-Intensive-Capstone-Project
 This project demonstrates the development of a Data Automation Agent capable of automating the end-to-end process of dataset analysis and reporting. The agent pipeline includes data validation, cleaning, statistical analysis, and report generation, all powered by Google Gemini LLM and custom AI agents.

The motivation is simple: manual dataset evaluation and reporting are time-consuming and error-prone, especially for enterprise-level datasets. This agent ensures faster insights, reproducibility, and structured reporting.

# DataFlow Automation Agent
## Problem Statement

Data analysts and teams spend hours manually validating datasets, generating summaries, and preparing reports for stakeholders. This process can be inconsistent, prone to human error, and difficult to scale.

# Objective:
Develop an AI agent that can:

⦁	Validate dataset quality (missing values, types, completeness).
⦁	Compute statistical summaries automatically.
⦁	Generate professional, human-readable reports.
⦁	Maintain session and memory for long-running operations.
⦁	Be easily deployed and reusable for multiple datasets.

## Solution Approach

The solution consists of multi-agent architecture:

# Coordinator Agent:
Orchestrates the workflow between cleaner, analyzer, and reporter agents.

# Cleaner Agent:
Performs missing value handling, type correction, and data normalization.

# Analyzer Agent:
Computes statistical summaries, identifies outliers, and generates insights.

# Reporter Agent:
Generates a professional report using Google Gemini LLM, now dynamically inserting the current date in every report.

## Environment Setup

Create a `.env` file in the root folder:


## Overview
This project is a **multi-agent AI system** designed for automating data workflows:
- **CleanerAgent**: Validates and cleans datasets.
- **AnalyzerAgent**: Generates statistics and correlation insights.
- **ReporterAgent**: Uses Google Gemini API to produce a professional natural language report.
- **CoordinatorAgent**: Orchestrates the full pipeline.

## Features Implemented
- **Multi-Agent System**: Sequential & coordinated agent workflow.
- **Tools Integration**: Data cleaning, validation, statistics generation.
- **Sessions & Memory**: SessionManager for state, MemoryBank for long-term storage.
- **Observability**: Logging, tracing, metrics.
- **LLM Integration**: Google Gemini API for report generation.
- **Deployment**: Streamlit app for interactive use.

## Installation

```bash
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate     # Windows
pip install -r requirements.txt


