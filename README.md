<div align="center">  <img width="250" height="200" alt="ChatGPT Image Jan 7, 2026, 11_42_36 AM" src="https://github.com/user-attachments/assets/124f11db-6911-496f-b385-20a03759063b" /> </div>

# <div align="center"> Product Performance And User Journey Analysis</div>

## 1. Background and Overview

### Company Context
Alluring Cosmetics is a UK-based budget-friendly cosmetic brand operating a direct-to-customer e-commerce platform with a product catalog spanning 54,000 unique products serving 1.64 million customers. With a catalogue of 54,000 unique products and 1.64 million total visitors over the analysis period, the business has generated **£6.35 million** in total revenue.

Reporting to the Head of Product and Growth, this analysis  cover five months of behavioural event data - October 2019 to February 2020. It explores how users **acquire**, **activate**, and **retain** across the platform, with the goal of identifying what truly drives sustainable revenue growth.

### North Star Metric
#### Monthly Active Users (MAU)
The number of unique users completing at least one purchase per month.

### Supporting Metrics (Drivers of MAU Growth)
The following three metrics directly influence the MAU and form the analytical framework for this project:

- **User Conversion Rate** - % of users who complete a purchase
- **7-Day Activation Rate** - % of new users who purchase within 7 days of first arrival
- **90-Day Cohort Retention** - % of first-time buyers who return to purchase within 90 days of their first order
<br>

## 2. Data Structure and Overview
### Dataset Specifications
- Analysis Period: October 2019 - February 2020 (5 months)
- Total Events Analysed: 20 Million behavioural events
- Event Types: view, cart, remove_from_cart, purchase
- Unique Visitors: 1.64 Million customers
- Unique Products: 54,000 SKUs

### Data Schema
The analysis uses a consolidated event-level table combining all five months of data with the following structure:

<div align="center">  <img width="500" height="500" alt="ChatGPT Image Jan 2, 2026, 04_22_09 PM" src="https://github.com/user-attachments/assets/6a6c2dcc-52f0-4fc3-a0a4-d18d1d221fb3" /> </div>

### User Journey Types
Two distinct behavioural paths exist in the data:

| Segment | Behavioral Path | Analytics Summary |
| :--- | :--- | :--- |
| **Traditional Browsers** | `view` → `cart` → (`remove_from_cart`) → `purchase` | **97.6% of users (1.6M).** These users browse product pages before adding to cart.|
| **Direct-to-Cart Users** | `cart` → (`remove_from_cart`) → `purchase` | **2.4% of users (40K).** Arrive via marketing channels with no `view` event.|

<br>

## 3. Executive Summary

<br>

<img width="1013" height="540" alt="Screenshot 2026-02-19 171421" src="https://github.com/user-attachments/assets/27454448-1865-443a-a2c4-53fc3f44aec8" />

Revenue follows active purchasing users. When MAU increases, revenue increases. This makes **MAU the clearest indicator of demand strength**.
<table align="center">
  <tr>
    <div width="1000">
      <td width="500" valign="top">
        <ol>
          <li>
            <strong>Are Users Coming Back?</strong>
            <ul>
              <li>MAU peaked in November (31.5K) following strong acquisition. However, returning user percentage increased steadily from 0% in October to 31% in February.</li>
              <li>While total MAU declined after November, the  quality of the remaining active base improved. Growth shifted from campaign-driven to a more stable returning base.</li>
            </ul>
          </li>
          <li>
            <strong>Are Users Becoming More Valuable?</strong>
            <ul>
              <li>No. Average Order Value remained stable (~£5 per item). Items per user remained largely stable between 9 and 10 items monthly.</li>
              <li>Revenue growth did not come from higher pricing or deeper monetization. It scaled primarily with the number of the active buyers.</li>
            </ul>
          </li>
        </ol>
      </td>
      <td width="500" valign="top">
        <ol start="3">
          <li>
            <strong>Is Growth Acquisition-Led or Retention-Led?</strong>
            <ul>
              <li>November's revenue spike was acquisition-led and campaign-driven. However, retention rates for subsequent cohorts suggest that promotional spikes have not yet translated into sustained compounding growth.</li>
              <li>The business responds well to campaigns but is still developing a steady retention strategy that works</li>
            </ul>
          </li>
          <li>
            <strong>90-Day Retention Context</strong>
            <ul>
              <li>28.7% of first-time buyers return within 90 days (Oct–Nov cohorts). October's 32% retention outperformed November's 25%, suggesting that buyers acquired through intent not promotion retain better. Expanding the returning user base is the clearest path to sustainable revenue growth. </li>
            </ul>
          </li>
        </ol>
      </td>
    </div>
  </tr>
</table>

**Strategic Insight**
<br>Alluring Cosmetics can scale revenue quickly through acquisition campaigns. However, sustainable growth depends on strengthening post-purchase engagement and increasing the proportion of returning active users. The way forward is not simply more traffic, but rather more repeat behaviour.

### Key Findings at a Glance
#### 1. User Conversion Rate
##### Segmented Conversion Performance:
Overall conversion rate is 6.92%, but Direct-to-Cart users convert at 12.04%, nearly double the 7% conversion of traditional browsers, highlighting the strong impact of targeted marketing channels.

##### High Cart Abandonment:
78% of all 'Add to Cart' events fail to reach the checkout stage, with the 'Remove from Cart' event rate (70%) significantly exceeding industry benchmarks. This indicates high transactional volatility, where more than half of intent-signals are being actively reversed, leading to substantial revenue leakage.

##### Behavioural and Pricing Insights:
Converting users explore 38 products vs 4 for non-converters, indicating substantial product comparison is required for purchase.
Items removed from the cart (£5.23) are slightly more expensive than purchased items (£4.93), suggesting relative price sensitivity as a potential growth lever.

#### 2. 7-Day Activation Rate 
The 7-day activation analysis reveals that only **5% of new users** complete their first purchase within the first week of arrival at Alluring Cosmetics. The data confirms that the first seven days, particularly the first 24 hours, represent the make-or-break window for converting new visitors into customers. While this rate sits within typical cosmetics e-commerce benchmarks (3-8%), it masks significant performance variation across user segments and a concerning 33% decline from peak to trough over the five-month period.

#### 3. 90-Day Cohort Retention
Overall, the 90-day cohort analysis shows a **28.7% retention rate**, with 15K of 53K first-time buyers returning to purchase, and clear monthly cohort variation, with October outperforming November by 28% (32% vs 25%), indicating seasonal or promotional effects. While Direct-to-Cart users activate faster, retention quality is materially higher among Traditional Browsers (30% vs 6%), and considered buyers (Day 1–7 activators) retain 57% better than Day 0 buyers, highlighting the trade-off between speed and long-term value.
<br>

## 4. Insight Deep Dive

## <div align="center"> User Conversion Rate: Two Distinct User Journeys </div>

The overall conversion rate is 6.92%. This single number masks a significant behavioural split between traditional browse-to-purchase path and Direct-to-cart user, which is reflected in their separate conversion rates.

|<img width="1023" height="573" alt="Screenshot 2026-01-11 183245" src="https://github.com/user-attachments/assets/de5d8edb-ab3e-433b-97f9-6b900eefddfd" />|<img width="959" height="537" alt="Screenshot 2026-01-11 184342" src="https://github.com/user-attachments/assets/13a40685-484e-4b36-bfa3-9bb58c4794e2" />|
| -------- | -------- |
| **Traditional Browsers (The Core Audience)**: <br> This segment of 1.6M users follow the expected e-commerce journey: View → Cart → Purchase . The 7% conversion rate sits at the higher end of the typical 2-5% cosmetics e-commerce benchmark, suggesting the product pages and browsing experience effectively communicate value. However, the real challenge emerges at the cart stage, among those who add items to cart, a substantial majority abandon without completing purchase (78%). |  **Direct-to-Cart Users:** <br> Also called The High-Intent Segment. This smaller cohort of 40K users exhibits dramatically different behaviour. By arriving directly at cart through targeted channels, they demonstrate higher purchase intent from the outset. The 12% conversion rate, nearly double that of traditional browsers, validates the effectiveness of email marketing and social media strategies. These users have already been pre-sold through marketing content, requiring less persuasion at the product page level (88%). This segment represents only 2.4% of total traffic. Growing it from 2.4% to even 5% would deliver disproportionate conversion gains without requiring platform-wide changes.| 

#### 1.1 The Cart Abandonment Challenge
Of all users who add items to cart , **72%** fail to complete the transaction. This represents not just lost revenue but wasted acquisition cost, implying the brand has successfully attracted and engaged these users, only to lose them at the final hurdle.

Breaking down this 72% abandonment reveals two distinct user behaviours:

<img width="647" height="226" alt="Screenshot 2026-02-17 124934" src="https://github.com/user-attachments/assets/ab731fc8-f01f-4af4-ae9a-e40bf7b66e16" />

#### 1.1a Active Removal: 46% Explicit Remove Rate
Almost half of cart users actively click "remove" to delete items, representing a conscious decision to reverse their initial purchase intent. This 46% rate far exceeds the 15-30% industry norm for active removals, suggesting issues in value perception rather than platform usability.

The **analysis of removed products** provides insight into average removed product price -  £5.23 (removed products) vs. £4.93 (purchased products) - a 6% price difference. These products are not expensive in absolute terms. The issue is not price shock but relative value perception. Users add items during browsing, then on reviewing or comparing options in their cart total, decide the value proposition is not compelling enough.

Contributing **factors that drive active removal** likely include: high shipping costs, cart used as a comparison tool, and unmet promotional expectations. 

#### 1.1b Passive Abandonment: 26% Leave Without Action
Users add items to cart but leave without taking any action — no removal, no purchase. This is likely driven by session timeouts, interruptions, or deferred decision-making. The relatively low passive abandonment rate (26% vs. 46% active) actually indicates that the problem isn't user distraction or checkout friction; users are actively choosing not to buy rather than passively forgetting. The intervention required is at the value and decision stage — not at checkout.

#### 1.2 Monthly Conversion Trends

<img width="1471" height="407" alt="Screenshot 2026-02-16 150926" src="https://github.com/user-attachments/assets/9dbe4e13-58d3-424c-b738-1895d159b5ce" />

**November 2019** stands out as the **best-performing** month with an 8.86% conversion rate and the **lowest cart abandonment** across the period. This represents a 33% improvement over October's 6.63% conversion rate. Additionally, the 4.65 point reduction in cart abandonment from October to November suggests an external factor driving performance: Black Friday/Cyber Monday promotions, Holiday shopping season, free shipping thresholds.

Understanding what drove November's outperformance could inform strategies to replicate that success in other months. Conversely, October's 80.07% cart abandonment, the worst performance, requires an investigation into whether it represents a seasonal baseline or a specific issue that month.

December through February cluster at a stable 6.79 – 7.15% conversion rate, suggesting this is the platform's true baseline when no promotional factor is active. November is an instructive outlier, not the norm. The strategic question is: what specifically drove November's performance, and can it be replicated outside of Black Friday season?

## <div align="center">  7-Day Activation Rate </div> 

<div align="center">  <img width="800" height="400" alt="Screenshot 2026-01-22 195145" src="https://github.com/user-attachments/assets/e450bd6e-372d-4a6b-ab07-3656dda67ddd" /> </div>
<br>
The **7-day activation analysis** reveals that only **5% of new users** complete their first purchase within the **first week of arrival** on the platform. While this sits within the typical cosmetics e-commerce benchmark (3-8%), it masks significant variation across Traditional browsers and Direct-to-Cart users as seen below.

#### 2.1 Two User Journeys, Vastly Different Outcomes 

<img width="550" height="352" alt="Screenshot 2026-01-24 231210" src="https://github.com/user-attachments/assets/cb1e0178-158f-4e16-9e4e-7c7039145314" />

The 2.4x performance advantage of Direct-to-Cart users validates current email marketing and social commerce strategies. 
These users arrive pre-qualified—marketing content has already communicated product value, addressed objections, and built purchase intent before they reach the website. The platform simply needs to facilitate the transaction, not persuade them to buy.

#### 2.2 The First Week is Make-or-Break
<img width="550" height="556" alt="Screenshot 2026-01-25 162728" src="https://github.com/user-attachments/assets/9d908be1-d73e-4def-a064-b5704138152c" />

Examining when users make their first purchase after initial arrival reveals stark urgency patterns. Of all users who eventually purchase, 84% complete their first transaction within 7 days of their first platform interaction. 
The remaining 16% purchase between days 8-30, with virtually no purchases occurring beyond 30 days. Users who don't purchase within the first week are overwhelmingly unlikely to convert at all, the platform has one week to convince new visitors of value before losing them permanently.

#### 2.3 Day 0 Dominates
<img width="658" height="360" alt="Screenshot 2026-02-10 161309" src="https://github.com/user-attachments/assets/c0b42875-2408-48e6-8359-522b82a0f6fe" />

Within the 7-day activation window, purchase timing concentrates heavily on Day 0 (same calendar day as first arrival). Of the 80,367 users who activated within 7 days, 57K (80%) purchased on Day 0 itself.
The first-hour experience must be optimized for immediate conversion. Friction in product discovery, cart processes, or checkout during this window directly impacts activation rates. Mobile experience is particularly critical, as impulse purchases disproportionately occur on mobile devices.

## <div align="center"> 90-Day Cohort Retention </div>


<div align="center"> <img width="601" height="338" alt="Screenshot 2026-02-07 234352" src="https://github.com/user-attachments/assets/92bfd1b2-db49-4892-82e3-9949555145de" /> </div>


28.67% of first-time buyers return to make a second purchase within 90 days of their initial transaction, sitting perfectly within the typical cosmetics e-commerce benchmarks (15-30%). A further breakdown of retention quality across acquisition channels and purchase timing is seen below.

#### 3.1 The Retention Curve

<img width="640" height="452" alt="Screenshot 2026-02-08 233637" src="https://github.com/user-attachments/assets/759e95e0-77fc-4fcc-85e8-efda322e68f6" />

##### What the Curve Reveals
The observed 90-day retention pattern reflects a mix of transactional behaviour and genuine repeat demand, rather than a simple loyalty progression. Early repurchases **(Days 0–7, 7.03%)** are best interpreted as post-purchase corrections and operational follow-ups, while the strongest growth between **Days 8–30 (+10.15pp)** aligns with the first realistic repurchase window driven by product depletion and lifecycle marketing exposure. **Beyond Day 60**, retention flattens, indicating that most repeat demand has already happened, and that the remaining repurchasers represent a smaller, high-intent segment - making this window more valuable for identifying true long-term customers than for driving incremental volume.

#### 3.2 Cohort Performance: October's 32% vs November's 25%
<img width="467" height="356" alt="Screenshot 2026-02-09 162020" src="https://github.com/user-attachments/assets/0bf28329-3ca2-44a7-80ed-5a0c9c2d269d" />

The October cohort outperformed November on 90-day retention (32% vs 25%) despite having fewer first-time buyers, indicating that October acquired higher-quality customers, while November scaled volume at the expense of retention efficiency.

**Why October May Have Performed Better**
- October buyers likely represent planners, customers shopping ahead of the holiday rush rather than reacting to discounts. This group tends to be more intentional, less price-sensitive, and more aligned with long-term brand value, which translates into stronger repeat-purchase behaviour.
- October purchases were more likely driven by product appeal (shade match, formulation, reviews) rather than price incentives. November’s Black Friday environment typically attracts deal-seekers whose primary motivation is discount depth, not brand affinity, lowering retention despite higher acquisition volume.
- October purchasers had their entire 90-day window during peak holiday season (Oct-Jan), potentially benefiting from gifting occasions and seasonal product relevance. November buyers' windows (Nov-Feb) include post-holiday months with reduced cosmetics purchase motivation.

#### 3.3 Retention by User Type: Traditional v Direct-to-Cart

<img width="515" height="245" alt="Screenshot 2026-02-10 162938" src="https://github.com/user-attachments/assets/419cc9c0-0919-4d5c-9d0e-5a999e972d50" />

**Understanding the Difference in Behaviour**
- Self-Directed Discovery Creates Commitment: Traditional Browsers by nature tend to spend time exploring the product catalog, viewing images, and comparing options. This creates understanding and commmitment to their purchase. Further re-enforcing their slower time to activate, reflecting deliberation which is correlated to satisfaction and viewing images, and repurchase intent. Additionally, users who find Alluring Cosmetics through their own discovery journey demonstrate intrinsic interest in the brand or product category, not just response to promotional stimulus.
- Campaign-Driven Intent is Transactional: Direct-to-Cart users arrive via email campaigns, social media ads, or promotional links with pre-loaded carts. Triggering purchases by marketing efforts. Leading to users with weak brand loyalty, who lack motivation to return at full price. Finally, because Direct-to-Cart users also tend to bypass browsing and validating their choice against other options, they face the risk of lower satisfaction if the promoted product doesn't meet expectations.


#### 3.4 Repurchase Timing

<img width="700" height="433" alt="Screenshot 2026-02-13 124130" src="https://github.com/user-attachments/assets/f37d5674-4382-4141-ac8a-c759554eddf8" />


Examining when repeat purchases occur within the 90-day window reveals concentration in the earliest days, with a rapid decay pattern suggesting distinct behavioural segments.

##### Time to Second Purchase Distribution
**- Day 0 (Same-Day Repurchase): 1,349 users**
Same-day repurchase is not retention; rather, it is a diagnostic metric for transactional behaviour and checkout experience. This behaviours could be driven by Cart Splitting for Free Shipping (customers seeking to exploit multiple promotions), check-out session timeouts, immediate uppsells and payment method switching. Industry benchmarks for checkout frictionsuggest 1-3% is normal, so Alluring Cosmetics is within expected range of 2.4% of day 0 repeat purchases, howvever, extension of session timeouts and earlier timing in upsells can be implemented.

**- Days 1–10 ( Rapid Engagement / Early Satisfaction): 2,896 users**
These users are likely driven by high satisfaction with the first product, gifting, or small corrections (wrong shade, size, or minor cart adjustments). Some may be influenced by impulse or promotional triggers, so not all purchases indicate “true retention.”

These users are high-value early adopters, and opportunities exist for engagement with loyalty programs, cross-sells, or VIP campaigns to capture early enthusiasm and reinforce brand affinity.

**- Day 11–20: (Early Replenishment / Product Familiarization): 2, 487 users**
This represents  users starting first natural product usage and replenishment cycles. Stronger signal of product satisfaction, as these users are repurchasing after experiencing the product rather than immediately reacting to UX or promotions.

Critical window for reinforcing product experience through personalized recommendations and retention messaging.These users are potential repeat customers, likely to stick if the first product meets expectations.

**- Day 21–90: (True Retention / Replenishment Window): 8,224 users**
This aligns with natural cosmetic usage cycles (e.g., mascara, foundation, skincare), reflecting actual satisfaction-driven repurchase behavior. Users in this window are more likely purchasing based on experience with the first product rather than brand curiosity or short-term impulse. This window captures real product-level retention and the formation of repeat customers. And it is a key focus for measuring brand loyalty, product satisfaction, and replenishment behavior.

A strategic focus on customer experience, replenishment reminders, and retention campaigns to maximize LTV.

 
**Recommendation:** Direct-to-Cart users need post-purchase engagement to convert them into retained customers. Email sequences, educational content, and product recommendations could bridge the retention gap.


## 5. Recommendations

Based on the analysis findings, the following actionable items can be prioritized by Alluring Cosmetics:

### 5.a Conversion Funnel
#### Scale Direct-to-Cart Channels Given 12% Conversion Advantage
Direct-to-cart users convert more. Alluring Cosmetics should lean into it.
- Expand email product campaigns -Send more product-focused emails with clear Add to Cart buttons. These users already have intent. Make acting on it easy.
- Increase social media product tagging- Tag more products in posts and stories. Let users shop without leaving the feed or browsing multiple pages.
- Enhance recommendation widgets - Add Quick Add to Cart buttons on homepage, category pages, and post-purchase screens. Capture impulse decisions in the moment.
#### Reduce Active Removal Through Improved Value Transparency
- Implement exit-intent intervention - When users attempts to remove item, trigger popup: "Wait! Here's 10% off this item" or "Customers also bought cheaper alternative instead." Test message variants for effectiveness.
- Add social proof at cart stage - Display "127 people bought this today" or "4.5★ based on 1,234 reviews" for items in cart. Reinforces purchase decision when users are wavering.
#### Implement Cart Recovery Campaign for Passive Abandoners
- Automated email sequence - Email #1 at 1 hour: "You left items in your cart." Email #2 at 24 hours: "Still interested? Cart expires soon." Email #3 at 72 hours: "Last chance—complete your order."
- Include product images and direct checkout link - Show exact items left in cart with prices and "Complete Purchase" button going straight to checkout.
- Test incentive in final email - A/B test with vs. without 10% discount in 72-hour email to measure incremental conversion vs. margin impact.

### 5.b 7-Day Activation Rate 

Users who do not purchase in the first 7 days are very unlikely to convert later. The first week is the make-or-break window. If we do not win them early, we lose them.

#### Scale Direct-to-Cart Acquisition Channels (12% Activation Rate)
- Direct-to-Cart users activate at 12%, more than double Traditional Browsers at 5%. Growing this segment from 2.5% to 5% of traffic delivers disproportionate activation gains. This can be achieved by expanding **email product campaigns**, **increasing social commerce product tagging**, and **implementing influencer affiliate program**.

#### Optimize First-Hour Conversion Experience
- 80% of Day 0 purchases occur within 1 hour of first arrival. This impulse window represents the highest-conversion opportunity but also the highest-friction risk. It should be well protected. It can be optimised through the **implementation of exit-intent intervention**, **reduced checkout friction**, **optimized mobile experience**.

### 5.c 90-Day Cohort Retention

#### Optimize the Day 8-30 Retention Window (60% of Retention Formation Occurs Here)

The retention curve shows steepest growth from Day 7 (7%) to Day 30 (17%), adding 10 percentage points. This is the critical window where most loyalty is formed. The goal is to convert undecided users with targeted incentive during this last high-conversion window.
- Implement "How's It Going?" Check-In Email Trigger 10 days after first purchase.
- For Fast-Consumption Products with predictable depletion, send Replenishment Reminder emails on Day 21. This should show product image, direct reorder link and discount on recurring orders
- Before momentum fades, send a time-bound offer for first-time buyers. Personalize recommendations based on what they bought. Create urgency but keep it credible on Day 30.

#### Investigate and Replicate October Cohort's 32% Retention Success

October 2019 cohort retained 32% versus November's 25%, a 28% performance gap.
- Compare Marketing Channel Mix (October vs November). Was October more organic? Less discount heavy? Higher intent traffic? Identify what brought better customers. 
- Review promotions and pricing (if any). Did November Black Friday/Cyber Monday affect behaviour? Were discounts too aggressive? Did free shipping thresholds change?
- Analyze Product Mix Purchased. Did October buyers purchase different product categories? Product quality or satisfaction differences? 
- Assess Traffic Source Quality and Referral sources, Paid vs organic ratio Geographic or demographic shift.
October’s performance suggests that how customers are acquired matters more than how many are acquired. Scaling via promotions can inflate top-of-funnel growth, but sustainable revenue is driven by cohorts acquired through product-driven intent, not discount urgency.

#### Bridge the Direct-to-Cart Retention Gap (6% → Target 15%)
Direct-to-Cart users activate efficiently (12% rate) but retain poorly (6%), representing acquisition investment with minimal lifetime value return.
- Implement Post-Purchase Education Sequence for Direct-to-Cart Buyers Within 24 hours of first purchase to build connection.
- Segment Direct-to-Cart Users by Campaign Source: Not all Direct-to-Cart traffic is equal, then analyse retention by campaign type: Email subscribers (likely higher intent), Social media ads (possibly lower quality), Influencer affiliate links (depends on influencer-brand alignment) etc
- Test Hybrid Journey: Campaign Landing → Browsing Encouraged. Instead of campaign emails with direct "Add to Cart" links, test landing users on curated collection/bundles pages

#### Reduce Day 0 Repurchase Friction (Diagnostic Improvement)
1,349 users (2.4% of first-time buyers) make a second purchase on the same day as their first - signaling potential checkout or merchandising friction. This is Not Retention: Day 0 repurchase measures transactional issues, not loyalty.  However, reducing friction improves customer experience and potentially converts split purchases into larger single orders.







