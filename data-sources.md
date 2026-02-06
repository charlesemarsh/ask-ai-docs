---
layout: default
title: Data Sources
---

# Data Sources

<p class="lead">Ask AI - Data Connector supports 14 data source integrations across three plan tiers.</p>

## Shopify <span class="badge badge-free">Free</span>

Your store's orders, products, collections, customers, and inventory data. Syncs automatically when you install the app.

**Resources synced:**
- **Orders** — Order history and transaction data (ID, date, status, totals, line items, shipping/billing country)
- **Products** — Product catalog and variants (title, description, vendor, SKU, price, inventory)
- **Collections** — Product collections and smart collections
- **Customers** — Customer records and purchase history (anonymized ID, order count, total spent, country)
- **Inventory** — Stock levels across locations
- **Abandoned Checkouts** — Cart abandonment and recovery data
- **Traffic** — Session and visitor data (requires Shopify Plus)

**Example questions:**
- "How's my revenue this month compared to last month?"
- "What are my top selling products?"
- "Show me orders by country"
- "Which customers have the highest lifetime value?"
- "What's my cart abandonment rate this week?"

---

## Klaviyo <span class="badge badge-pro">Pro</span>

Email and SMS marketing automation platform.

**Resources synced:**
- **Email Campaigns** — Campaign ID, name, subject lines, send dates, status, performance metrics (open rate, click rate, conversions), revenue attribution
- **Automated Flows** — Flow ID, name, status, trigger types (abandoned cart, welcome series, etc.), performance metrics
- **Subscriber Lists** — List/segment names, subscriber counts, created/updated dates

**How to get your API key:**
1. Log in to your Klaviyo account
2. Click your account name (bottom left) > Settings
3. Navigate to "API Keys" in the left sidebar
4. Click "Create Private API Key"
5. Name it (e.g., "Ask AI - Data Connector")
6. Select read-only access to Campaigns, Flows, and Lists & Segments
7. Click "Create" and copy the key

<div class="callout callout-warning">
Only grant read-only permissions. Ask AI - Data Connector never needs write access to your Klaviyo account.
</div>

**Example questions:**
- "Which email campaigns have the highest open rate?"
- "Show me my flow performance metrics"
- "How many subscribers do I have across all lists?"
- "What's the revenue from my welcome series flow?"

---

## Recharge <span class="badge badge-pro">Pro</span>

Subscription management platform for recurring orders.

**Resources synced:**
- **Subscriptions** — Active and cancelled subscriptions
- **Customers** — Subscription customer records
- **Charges** — Billing charges and transactions

**How to get your API key:**
Go to Integrations > API tokens in your Recharge dashboard to create an API token.

**Example questions:**
- "What's my MRR trend this quarter?"
- "Why are customers cancelling their subscriptions?"
- "How many active subscriptions do I have?"
- "What's my subscription churn rate?"

---

## Gorgias <span class="badge badge-pro">Pro</span>

Customer support helpdesk built for e-commerce.

**Resources synced:**
- **Support Tickets** — Ticket ID, subject, status, created/closed dates, response times, channel, tags, satisfaction ratings
- **Daily Stats** — Daily support performance metrics

**How to get your API key:**
1. Log in to your Gorgias account
2. Go to Settings (gear icon) > REST API
3. Click "Create API Key"
4. Name it (e.g., "Ask AI - Data Connector")
5. Set permissions to "Read-only"
6. Copy both the API Key (username) and API Secret (password)
7. You'll also need your Gorgias domain (e.g., yourstore.gorgias.com)

**Example questions:**
- "What's my average response time this week?"
- "How many support tickets did we receive today?"
- "What's our CSAT score trend?"
- "Show me ticket volume by channel"

---

## Microsoft Clarity <span class="badge badge-pro">Pro</span>

User experience analytics with session recordings, heatmaps, and behavior insights.

**Resources synced:**
- **UX Stats** — Daily session and engagement metrics

**Features:**
- Session analytics
- Rage click detection
- Dead click tracking
- Scroll depth analysis
- Device and browser breakdown

**How to get your API key:**
Go to Settings > Data Export in your Clarity project to generate an API token.

**Example questions:**
- "How many rage clicks did we have this week?"
- "What's our average session engagement time?"
- "Show me UX issues by device type"
- "What's the scroll depth on our landing pages?"

---

## YouTube <span class="badge badge-pro">Pro</span>

Video analytics, engagement metrics, and transcripts from your YouTube channel.

**Resources synced:**
- **Channel Data** — Channel statistics and metadata
- **Video Data** — Video details, stats, and transcripts

**Features:**
- Video performance tracking
- View and engagement analytics
- Video transcript extraction
- Chapter detection
- Daily stats snapshots
- Subscriber tracking

**How to connect:**
Connect your YouTube channel via OAuth to sync video data and transcripts.

**Example questions:**
- "What are my top performing videos?"
- "Show me views gained this week"
- "Which videos have transcripts?"
- "What's my subscriber count trend?"

---

## Reviews.io <span class="badge badge-pro">Pro</span>

Product reviews, ratings, and customer feedback analytics.

**Resources synced:**
- **Reviews** — Product reviews and ratings
- **Stats** — Daily review statistics and metrics
- **Survey Responses** — Customer survey feedback

**How to get your API key:**
Find your Store ID and API Key in your Reviews.io dashboard under Integrations > API.

**Example questions:**
- "What's my overall store rating?"
- "Show me recent reviews"
- "Which products need more reviews?"
- "What's my review sentiment this month?"

---

## Yotpo <span class="badge badge-pro">Pro</span>

Product reviews, ratings, and user-generated content analytics.

**Resources synced:**
- **Reviews** — Product reviews and ratings
- **Product Stats** — Aggregated review stats by product

**How to get your API key:**
Find your Store ID and API Secret in your Yotpo dashboard under Account Settings > Store Setup.

**Example questions:**
- "What's my average product rating?"
- "Show me review trends this month"
- "Which products have the lowest ratings?"
- "How many verified buyer reviews do I have?"

---

## Smile.io <span class="badge badge-pro">Pro</span>

Loyalty and rewards program analytics for customer retention.

**Resources synced:**
- **Members** — Loyalty program members and VIP status
- **Points Transactions** — Points earned and redeemed
- **VIP Tiers** — VIP tier definitions and perks

**How to get your API key:**
Find your API key in your Smile dashboard under Settings > Developer tools > Manage API keys.

**Example questions:**
- "How many loyalty members do I have?"
- "What's the points redemption rate?"
- "Show me VIP tier distribution"
- "What's the engagement rate of my loyalty program?"

---

## Swish <span class="badge badge-pro">Pro</span>

Wishlist analytics showing product demand and customer purchase intent.

**Resources synced:**
- **Wishlist Items** — Products saved to customer wishlists
- **Wishlists** — Customer wishlist collections

**How to get your API key:**
Find your API key in your Swish dashboard under Settings > Developer tools > Manage API keys.

**Example questions:**
- "What are the most wishlisted products?"
- "How many items are on wishlists?"
- "Which products have the highest demand?"
- "Which variants are most popular?"

---

## Google Analytics 4 <span class="badge badge-business">Business</span>

Website traffic, user behavior, and conversion tracking from GA4.

**Resources synced:**
- **Traffic Data** — Daily sessions, users, and engagement metrics

**Features:**
- Session and user tracking
- Traffic source analysis
- Device and browser breakdown
- Geographic data
- Conversion tracking
- Engagement metrics

**How to connect:**
Connect your verified GA4 property via OAuth to see website traffic and user behavior data.

**Example questions:**
- "How many users visited my site this week?"
- "What are my top traffic sources?"
- "Show me sessions by device type"
- "What's my bounce rate trend this month?"

---

## Google Search Console <span class="badge badge-business">Business</span>

Organic search performance data including keywords, clicks, and rankings.

**Resources synced:**
- **Search Stats** — Daily search performance metrics

**Features:**
- Keyword performance tracking
- Click and impression data
- Average position tracking
- CTR analysis
- Top landing pages

**How to connect:**
Connect your verified Search Console property via OAuth to see organic search data.

**Example questions:**
- "What are my top performing keywords?"
- "Show me my organic search traffic trends"
- "Which pages get the most search impressions?"
- "What's my average search position this month?"

---

## Triple Whale <span class="badge badge-business">Business</span>

Marketing attribution and ROAS analytics for e-commerce brands.

**Resources synced:**
- **Summary Metrics** — Daily revenue, ROAS, and marketing metrics
- **Attribution Data** — Order-level marketing attribution

**Features:**
- Marketing attribution tracking
- ROAS and MER calculations
- Channel performance analysis
- Customer journey insights

**How to get your API key:**
Generate an API key from your Triple Whale dashboard under Settings > API Keys.

<div class="callout callout-info">
You may need a paid Triple Whale plan with API access enabled.
</div>

**Example questions:**
- "What's my ROAS for the last 30 days?"
- "Which marketing channel has the best attribution?"
- "Show me my marketing performance trends"
- "What's my MER this month compared to last month?"
