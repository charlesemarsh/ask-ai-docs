---
layout: default
title: Privacy Policy
---

# Privacy Policy

<p class="lead">Ask AI - Data Connector is designed to provide analytics and insights without compromising customer privacy.</p>

*Last updated: February 2026*

## Overview

Ask AI - Data Connector ("we", "our", "the app") connects your e-commerce data sources to AI through the Model Context Protocol (MCP). This privacy policy explains what data we collect, how we use it, and how we protect it.

## What We Do NOT Store

We do not store personally identifiable information (PII):

- Customer names, email addresses, or phone numbers
- Full billing or shipping addresses
- Credit card or payment details
- IP addresses or device identifiers
- Email message content from campaigns
- Support ticket message contents

## What We DO Store

We store only the data necessary to provide analytics and insights:

- **Anonymized customer IDs** — For aggregate analysis only, not linked to personal information
- **Geographic data** — At country/region level only (no full addresses)
- **Transaction amounts and order metadata** — Order totals, discounts, taxes, shipping costs, and status
- **Product information** — Titles, descriptions, vendors, SKUs, prices, and inventory levels
- **Aggregated marketing and support metrics** — Campaign performance, flow stats, ticket counts, and response times

## Data Sources

When you connect third-party data sources (Klaviyo, Triple Whale, Gorgias, etc.), we sync only aggregated metrics and performance data. We do not access or store the underlying personal data from these platforms. See our [Data Sources]({{ '/data-sources/' | relative_url }}) page for a detailed breakdown of exactly what is synced from each provider.

## Google User Data

Our application integrates with Google services using OAuth 2.0 with **read-only** access. This section describes exactly what Google user data we access, how we use it, and how we protect it.

### Google Data Accessed

When you connect a Google service, we access only the following data:

| Google Service | OAuth Scope | Data Accessed |
|---|---|---|
| **Google Search Console** | `webmasters.readonly` | Organic search keywords, impressions, clicks, click-through rates, and average search position for your verified web properties |
| **Google Analytics 4** | `analytics.readonly` | Website sessions, users, page views, traffic sources, device and browser categories, and geographic data (country/region level only) |
| **Google Ads** | `adwords` (read-only) | Campaign names, impressions, clicks, cost, conversions, and performance metrics |
| **YouTube** | `youtube.readonly` | Channel statistics, video metadata (titles, descriptions, publish dates), view counts, engagement metrics (likes, comments), and video transcripts |

All Google API scopes are requested as **read-only**. Our application does not modify, delete, or create any data in your Google accounts.

### Google Data Usage

Google user data is used exclusively to:

- Display analytics dashboards within your Shopify admin so you can view marketing performance alongside your store data
- Enable AI-powered insights by making your analytics data queryable through the Model Context Protocol (MCP)
- Provide aggregated performance metrics and trend analysis across your connected data sources

Google user data is **not** used for:

- Advertising, remarketing, or ad targeting purposes
- Sale, rental, or transfer to third parties
- Training machine learning or AI models
- Profiling, tracking, or building user profiles
- Any purpose unrelated to providing the app's core analytics functionality

### Google Data Storage

- Google OAuth tokens (access and refresh tokens) are encrypted at rest using **AES-256-GCM** encryption and stored in our PostgreSQL database
- Synced analytics data (metrics, keywords, video stats) is stored in our database and associated with your Shopify shop
- Data retention follows your subscription tier: 7 days (Free), 90 days (Pro), unlimited (Business)
- All data is encrypted in transit via TLS/HTTPS

### Google Data Sharing

Google user data is **not shared** with any third parties. Data remains within our application infrastructure and is only accessible to the authenticated Shopify store owner who connected the Google account.

When you use the MCP endpoint to query your data via an AI client (such as Claude Desktop), the relevant analytics data is sent to the AI client you have configured. This is initiated by you and only occurs when you explicitly query your data.

### Revoking Google Access

You can disconnect any Google service at any time from the Data Sources page in the app. Upon disconnection:

- OAuth tokens are immediately revoked with Google and deleted from our database
- Synced data associated with that connection is removed
- You can also revoke access directly from your [Google Account permissions page](https://myaccount.google.com/permissions)

Upon app uninstallation, all Google user data and OAuth tokens are permanently deleted.

### Google API Services User Data Policy

Our use and transfer to any other app of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.

## Data Security

- All data is encrypted in transit using TLS
- All data is encrypted at rest
- API keys are stored securely and never exposed after initial creation
- We use industry-standard security practices for data storage and access

## Data Retention

- Your data is retained for as long as your app subscription is active
- Data history varies by plan (7 days for Free, 90 days for Pro, unlimited for Business)
- When you uninstall the app, your data is scheduled for deletion

## Data Deletion

- When a customer requests deletion through Shopify's privacy webhooks, we automatically remove all associated data
- You can uninstall the app at any time to trigger data cleanup
- You can contact us to request manual data deletion

## Compliance

We comply with:

- **GDPR** (General Data Protection Regulation)
- **CCPA** (California Consumer Privacy Act)
- **Shopify's data protection requirements** for app developers
- **[Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy)**, including the Limited Use requirements

## Third-Party Services

We integrate with the following categories of third-party services:

- **Shopify** — Your store data is accessed through Shopify's API with the permissions you grant during installation
- **Google services** — Google Search Console, Google Analytics 4, Google Ads, and YouTube data is accessed via OAuth 2.0 with read-only scopes. See [Google User Data](#google-user-data) above for full details
- **Third-party integrations** — Data from Klaviyo, Triple Whale, Gorgias, and other connected services is accessed using the API keys you provide
- **AI clients** — When you use the MCP endpoint, your data is sent to the AI client you've configured (Claude Desktop, Claude Code, etc.)

## Your Rights

You have the right to:

- **Access** your data through the app's dashboard and AI queries
- **Delete** your data by uninstalling the app or contacting us
- **Restrict** data collection by disconnecting specific data sources
- **Port** your data by exporting it through the app

## Changes to This Policy

We may update this privacy policy from time to time. Changes will be posted on this page with an updated revision date.

## Contact

If you have questions about this privacy policy or your data, please contact us through the Shopify App Store listing.
