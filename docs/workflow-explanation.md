
# Workflow Explanation

## Overview

The AI Daily Intelligence Automation is built using Make.com. It collects information from multiple AI news sources, processes the information using Google Gemini, and distributes the results through Gmail and Telegram.

## 1. RSS Feed Collection

The workflow starts with three RSS feed modules:

- OpenAI
- Google AI
- TechCrunch

Each module retrieves available news articles from its respective source.

## 2. Text Aggregation

Text Aggregators combine the collected RSS information into consolidated text inputs.

This makes it easier to send the collected information to the AI model for processing.

## 3. Google Gemini Processing

The aggregated news is passed to Google Gemini.

Two separate Gemini modules are used:

### Gmail Processing

Generates a detailed HTML newsletter containing AI news updates and relevant explanations.

### Telegram Processing

Generates a shorter, concise report formatted for Telegram delivery.

## 4. Router

A Make.com Router divides the workflow into two separate routes.

### Route 1: Gmail

Google Gemini → Gmail

Generates and sends the detailed AI newsletter.

### Route 2: Telegram

Google Gemini → Telegram Bot

Generates and sends the concise AI news report.

## 5. Scheduled Execution

The scenario is configured to run automatically every day at 8:00 AM.

## Complete Workflow

RSS Feeds
    ↓
Text Aggregators
    ↓
Google Gemini
    ↓
Router
   ↙   ↘
Gmail  Telegram
