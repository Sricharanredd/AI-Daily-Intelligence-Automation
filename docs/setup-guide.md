
# Setup Guide

## Prerequisites

Before recreating this automation, you need:

- A Make.com account.
- Access to Google Gemini through a supported Make integration.
- A Gmail account.
- A Telegram account.
- A Telegram bot created using BotFather.

## Step 1: Create a Make.com Scenario

1. Sign in to Make.com.
2. Create a new scenario.
3. Add the required RSS modules.
4. Configure the RSS feed URLs for your selected AI news sources.

## Step 2: Configure Text Aggregators

Add Text Aggregator modules to consolidate the information retrieved from the RSS feeds.

Configure the source modules and the fields required by your workflow.

## Step 3: Configure Google Gemini

Connect your supported Google Gemini integration.

Create two Gemini processing modules:

- One for generating the detailed Gmail newsletter.
- One for generating the concise Telegram report.

Use the prompt templates available in the `prompts/` directory.

## Step 4: Configure the Router

Add a Router module after the aggregation stage.

Create two routes:

- Route 1: Google Gemini → Gmail
- Route 2: Google Gemini → Telegram Bot

## Step 5: Configure Gmail

Connect your Gmail account and map the generated newsletter content into the email body.

Configure the required email fields and HTML formatting.

## Step 6: Configure Telegram

1. Create a Telegram bot using BotFather.
2. Connect the bot to Make.com.
3. Select the destination chat.
4. Map the generated report to the Telegram message field.
5. Configure HTML parsing if using HTML-formatted messages.

Never publish your bot token or credentials.

## Step 7: Configure Scheduling

Configure the Make.com scenario to execute daily at 8:00 AM.

## Step 8: Test the Automation

1. Execute the scenario using Run once.
2. Verify the Gmail newsletter.
3. Verify the Telegram report.
4. Check the execution history for successful completion.
5. Enable the scenario and verify its scheduled execution.

## Important Notes

This repository documents the workflow and provides prompt examples. It does not contain the private Make.com connections or credentials.

Recreating the automation requires configuring your own accounts and integrations.
