<div align="center">  <img width="200" height="200" alt="ChatGPT Image Jan 7, 2026, 11_42_36 AM" src="https://github.com/user-attachments/assets/124f11db-6911-496f-b385-20a03759063b" /> </div>

# <div align="center"> Product Performance And User Journey Analysis: A Funnel Optimization for E-Commerce </div>

## 1. Background and Overview

### Company Context
Alluring Cosmetics is a UK-based cosmetics brand operating an e-commerce platform with a product catalog spanning 54,000 unique products serving 1.64 million customers. 
The brand has generated **£6.35 million** in total revenue across its marketplace.

Reporting to the Head of Product and Growth, this project is in-depth analysis of Alluring Cosmetics' e-commerce performance over five months **(October 2019 - February 2020)**. 
The goal is to understand user behavior patterns across the full purchase journey, from initial product discovery through conversion to identify friction points, quantify drop-off rates, 
and uncover opportunities to drive sustainable growth. Translating **20 million user events** into actionable insights that inform product development, growth strategy, and monetization decisions. 

### North Star Metric
#### Monthly Active Purchasers (MAP)
The number of unique users completing at least one purchase per month. 


### Supporting Metrics (Drivers of MAP Growth)
The following six metrics directly influence the North Star Metric and form the analytical framework for this project:

- User Conversion Rate - Percentage of users who view products and complete a purchase
- 7-Day Activation Rate - Percentage of new users making their first purchase within 30 days
- 90-Day Cohort Retention - Percentage of first-time buyers who return to purchase within 90 days
- Multi-Product Engagement Rate - Percentage of users purchasing from multiple product categories
- Power User Ratio - Percentage of users making 3+ purchases within 90 days
- Time Between Purchases – Shorter cycles = more frequent revenue.
- Revenue per Active User (RPAU) - Average revenue generated per purchasing user

## 2. Data Structure and Overview

### Dataset Specifications
- Analysis Period: October 2019 - February 2020 (5 months)
- Total Events Analyzed: 20 Million behavioral events
- Event Types Captured: view, cart, remove_from_cart, purchase
- Unique Users: 1.64 Million customers
- Unique Products: 54,000 SKUs

### Data Schema
The analysis uses a consolidated event-level table combining all five months of data with the following structure:

<div align="center">  <img width="500" height="500" alt="ChatGPT Image Jan 2, 2026, 04_22_09 PM" src="https://github.com/user-attachments/assets/6a6c2dcc-52f0-4fc3-a0a4-d18d1d221fb3" /> </div>

## 3. Executive Summary

### Key Findings
#### 1. Conversion & Funnel Performance:
##### Segmented Conversion Performance:
Overall conversion rate is 6.92%, but Direct-to-Cart users convert at 12.04%, nearly double the 7% conversion of traditional browsers, highlighting the strong impact of targeted marketing channels.

##### High Cart Abandonment:
78% of all 'Add to Cart' events fail to reach the checkout stage, with the 'Remove from Cart' event rate (70%) significantly exceeding industry benchmarks. This indicates high transactional volatility, where more than half of intent-signals are being actively reversed, leading to substantial revenue leakage.

##### Behavioral and Pricing Insights:
Converting users explore 38 products vs 4 for non-converters, indicating substantial product comparison is required for purchase.
Items removed from the cart (£5.23) are slightly more expensive than purchased items (£4.93), suggesting relative price sensitivity as a potential growth lever.

#### 2. 7-Day Activation Rate 
The 7-day activation analysis reveals that only **5% of new users** complete their first purchase within the critical first week of arrival at Alluring Cosmetics. The data confirms that the first seven days, particularly the first 24 hours—represent the make-or-break window for converting new visitors into customers. While this rate sits within typical cosmetics e-commerce benchmarks (3-8%), it masks significant performance variation across user segments and a concerning 33% decline from peak to trough over the five-month period.


## 4. Insight Deep Dive

## <div align="center"> User Conversion Rate: Two Distinct User Journeys </div>

Analyzing conversion patterns revealed an important nuance: not all users follow the traditional browse-to-purchase path. While 97.6% of users (1.6M) engage in traditional product browsing, a smaller segment of 40,000 users (2.4%) add items directly to cart without viewing product pages first.



|<img width="1023" height="573" alt="Screenshot 2026-01-11 183245" src="https://github.com/user-attachments/assets/de5d8edb-ab3e-433b-97f9-6b900eefddfd" />|<img width="959" height="537" alt="Screenshot 2026-01-11 184342" src="https://github.com/user-attachments/assets/13a40685-484e-4b36-bfa3-9bb58c4794e2" />|
| -------- | -------- |
| **Traditional Browsers (The Core Audience)**: <br> This segment OF 1.6M users follow the expected e-commerce journey: View → Cart → Purchase . The 7% conversion rate sits at the higher end of the typical 2-5% cosmetics e-commerce benchmark, suggesting the product pages and browsing experience effectively communicate value. However, the real challenge emerges at the cart stage, among those who add items to cart, a substantial majority abandon without completing purchase (78%). |  **Direct-to-Cart Users:** <br> The High-Intent SegmentThis smaller cohort of 40K users exhibits dramatically different behavior. By arriving directly at cart through targeted channels, they demonstrate higher purchase intent from the outset.The 12% conversion rate—nearly double that of traditional browsers—validates the effectiveness of email marketing and social media strategies. These users have already been pre-sold through marketing content, requiring less persuasion at the product page level (88%).| 

#### 1.1 The Cart Abandonment Challenge: 70% of Users Never Purchase
Once users demonstrate purchase intent by adding items to cart, 70.53% fail to complete the transaction. This represents not just lost revenue but wasted acquisition cost—the brand has successfully attracted and engaged these users, only to lose them at the final hurdle.

Breaking down this 78% abandonment reveals two distinct user behaviors:
#### 1.1a Active Removal: 70% Explicit Remove Rate
More than half of cart users actively click "remove" to delete items, representing a conscious decision to reverse their initial purchase intent. This 54.49% rate far exceeds the 15-30% industry norm for active removals, suggesting systematic issues influencing user decision-making.

The **analysis of removed products** provides insight into average removed product price -  £5.23 (removed products) vs. £4.93 (purchased products). The 6% price difference tells us that products being removed aren't expensive in absolute terms—most are under £11. This suggests the issue isn't product price shock but rather relative value perception. Users add items to cart during browsing, but upon reviewing cart totals or comparing options, decide the value proposition isn't compelling enough. Factors that dirve active removal include the follwing - High shipping costs, cart used as a comparison tool, promotional expectations not met. 

#### 1.1b Passive Abandonment: 8.7% Leave Without Action
These users showed enough interest to add products but got distracted or deferred the decision. These users showed enough interest to add products but got distracted or deferred the decision. The relatively low passive abandonment rate (8.7% vs. 70% active) actually indicates that the problem isn't user distraction or checkout friction—users are actively choosing not to buy rather than passively forgetting. This reinforces that the core issue lies in the purchase decision itself, not the checkout process.

#### 1.2 Monthly Performance Trends
<img width="1468" height="401" alt="Screenshot 2026-01-08 172225" src="https://github.com/user-attachments/assets/91e6e901-d1da-4f53-a085-239e875fb047" />


November 2019 stands out with an 8.86% conversion rate and 75.42% cart abandonment—the best performance across both metrics. This 33% improvement over the October conversion rate (8.86% vs 6.63%) and 4.65 point reduction in cart abandonment suggests an external factor driving performance - Black Friday/Cyber Monday promotions , Holiday shopping season, free shipping thresholds.

Understanding what drove November's outperformance could inform strategies to replicate that success in other months. Conversely, October's 80.75% cart abandonment—the worst performance—requires an investigation into whether it represents a seasonal baseline or a specific issue that month.

The relative stability of December through February (6.79-7.15% conversion, apprx. 78% abandonment) suggests a baseline performance level when no exceptional factors are present, making November an instructive outlier rather than November being normal and other months being problematic.


## <div align="center">  7-Day Activation Rate </div>

The 7-day activation analysis reveals that only **5% of new users** complete their first purchase within the **first week of arrival** at Alluring Cosmetics e-commerce website. While this rate sits within typical cosmetics e-commerce benchmarks (3-8%), it masks significant performance variation across Traditional browsers and Direct-to-Cart users as seen below.

<img width="1032" height="266" alt="Screenshot 2026-01-22 195145" src="https://github.com/user-attachments/assets/e450bd6e-372d-4a6b-ab07-3656dda67ddd" />

## 5. Recommendations
Based on the analysis findings, the following actionable items can be prioritized by Alluring Cosmetics:

### 5.a Conversion Funnel

#### Reduce Active Removal Through Improved Value Transparency
- Implement exit-intent intervention - When user attempts to remove item, trigger popup: "Wait! Here's 10% off this item" or "Customers also bought [cheaper alternative] instead." Test message variants for effectiveness.
- Add social proof at cart stage - Display "127 people bought this today" or "4.5★ based on 1,234 reviews" for items in cart. Reinforces purchase decision when users are wavering.
#### Implement Cart Recovery Campaign for Passive Abandoners
- Automated email sequence - Email #1 at 1 hour: "You left items in your cart." Email #2 at 24 hours: "Still interested? Cart expires soon." Email #3 at 72 hours: "Last chance—complete your order."
- Include product images and direct checkout link - Show exact items left in cart with prices and "Complete Purchase" button going straight to checkout.
#### Scale Direct-to-Cart Channels Given 12.04% Conversion Advantage
- Expand email product campaigns - Increase frequency of emails featuring specific products with "Add to Cart" CTAs. Direct-to-cart users have already self-qualified their interest.
- Increase social media product tagging - Tag more products in Instagram/Facebook posts, creating shoppable content that bypasses product pages





