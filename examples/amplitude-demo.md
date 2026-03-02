# Amplitude Demo Transformation Case Study

## Company Background

Amplitude is an AI analytics platform offering event tracking, session replays, in-app guides, surveys, and web experiments.

## The Problem

Sales engineers were running 5-10 demos per week with:
- Spoofed analytics data from Google Sheets
- Only showing analytics, not full platform
- Generic demos for all prospects
- Manual data mapping process

For strategic enterprise accounts, generic demos weren't closing deals.

## The Solution

Custom demo websites + AI-powered user simulations:

### 1. Build Custom Demo Websites
Using AI coding tools (Claude Code, Cursor, Bolt) to create sites resembling prospect's actual product.

### 2. Define Customer Journeys
Relevant journeys like car buyers customizing vehicles, loyalty program visitors abandoning forms.

### 3. Browser Automation
Browserbase + Stagehand SDK to simulate realistic user behavior at scale.

### 4. Custom Logic Injection
Between AI-generated actions: produce event data, session replays, guides data, surveys.

### 5. Full Platform Demos
Analytics + session replays + guides + experiments + AI insights.

## Results

| Metric | Result |
|--------|--------|
| Custom demos built | 40+ |
| Simulated journeys | 5,600+ |
| Pipeline influenced | $10M+ |
| Adoption | Push → Pull (SEs requesting more) |

## Key Learnings

1. **Match the prospect's world** - Demo should feel like their product
2. **Show real journeys** - Not just happy paths
3. **Enable self-serve** - Remove bottlenecks
4. **Connect to pipeline** - Track demo impact in Salesforce

## Source

- [How Amplitude Transformed Sales Demos](https://www.browserbase.com/blog/how-amplitude-transformed-sales-demos-with-browser-automation)
