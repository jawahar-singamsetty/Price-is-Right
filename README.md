# 🛒 AI Deal Scanner & Price Estimator

## Overview

This notebook implements an **agentic AI pipeline** that **scans the internet for product offers**, estimates the **expected Amazon price** using a trained LLM-based price estimator, and **identifies potential deals** where the offer price is lower than the estimated Amazon price.

The goal is to automatically surface **real bargain opportunities** by comparing scraped prices against an AI-derived reference price.

---

## How It Works

The system follows a multi-step process:

1. **Scrape Offers Across the Internet**

   * Collects product offers from multiple online sources
   * Extracts structured data such as product description, price, and URL

2. **Estimate Amazon Price (AI-Powered)**

   * Uses a fine-tuned **LLM-based price estimator** trained on product descriptions
   * Predicts the expected Amazon-equivalent price for each product

3. **Deal Evaluation**

   * Compares the scraped offer price with the estimated Amazon price
   * Calculates the discount
   * Flags offers where the scraped price is **lower than the estimated Amazon price**

4. **Results Presentation**

   * Displays qualifying deals in a structured table
   * Includes description, scraped price, estimated price, discount, and source URL

---

## Key Features

* 🌐 Internet-wide deal scanning
* 🧠 LLM-based price estimation
* 💰 Automatic discount calculation
* 📊 Interactive results display (Gradio UI)
* 🤖 Agent-style orchestration with tool calls

---

## Technologies Used

* **Python**
* **Large Language Models (LLMs)**
* **Gradio** for interactive UI
* **Pydantic** for structured data validation
* **Agent-style tool calling** for modular execution

---

## Example Use Case

A user wants to find discounted products online:

* The system scans multiple websites for offers
* Estimates what the product should cost on Amazon
* Highlights only those deals where the offer price is cheaper than expected

This enables faster and more intelligent deal discovery than manual comparison.

---

## Output Example

| Description       | Offer Price | Estimated Amazon Price | Discount | URL  |
| ----------------- | ----------- | ---------------------- | -------- | ---- |
| iPhone 13 Pro Max | $699        | $799                   | $100     | link |

---

## Limitations

* Scraping depends on site availability and structure
* Estimated prices are **approximations**, not guaranteed Amazon listings
* Rare or niche products may have higher estimation error

---

## Intended Use

* Deal discovery and bargain hunting
* Price comparison automation
* Internal tools for e-commerce analysis
* Demonstrations of agentic AI workflows

---

## Author

**Jawahar S R**


