# Core Interview Cases

## 1. Third Wave Analytics Function

# Case Study 1 — Building Third Wave Coffee's Analytics Function

## Company / Business Context

Third Wave Coffee was a rapidly growing coffee retail chain with approximately 50–60 stores at the time.

The business was primarily offline / in-store, with a smaller share of revenue coming from:

- the Third Wave mobile app, which was used by only ~2–3% of customers,
- food-delivery platforms such as Zomato and Swiggy.

The business therefore generated data across multiple systems, but there was no unified analytics layer connecting these sources.

---

## My Role

I was the first dedicated analytics hire at Third Wave Coffee and reported directly to the CTO.

My mandate had two parts:

1. Deliver meaningful analytics output within the first 30/60/90 days using two vendor analysts from PwC.
2. Build an in-house analytics function over the following six months.

### Key Stakeholders

- Co-founder / leadership team
- CTO
- Product Lead
- Marketing Head
- Operations / Business teams
- Store and Area Managers

---

## Business Problem

The business lacked a consistent analytics layer and depended heavily on fragmented and manual reporting.

This created several problems:

- Leadership did not have a single, trusted view of business health.
- Different teams used different tools and metric definitions.
- Weekly business reporting required manual effort and typically had a turnaround time of 1–2 days.
- Marketing did not have an easy self-service mechanism for customer segmentation and campaign targeting.
- Product teams needed analytics support for experimentation and product-performance measurement.
- Ad-hoc requests consumed a disproportionate amount of limited analytics capacity.

A major underlying issue was that the same metric could mean different things to different teams. Metrics such as new customer, retention and ARPU were not centrally governed.

---

## My Responsibilities

I was responsible for:

- creating a single view of business health for the CXO / leadership team,
- creating role-specific analytical views for business, operations, product and marketing teams,
- standardizing key business metrics,
- establishing a repeatable analytics operating model,
- prioritizing incoming analytics requests,
- increasing self-service adoption,
- and building the internal analytics function.

---

## Baseline

When I joined:

- reporting was largely manual,
- the weekly business review required approximately 1–2 days of preparation,
- teams were working with separate tools and datasets in silos,
- there were approximately 4–5 major data sources:
  - POS data,
  - Swiggy data,
  - Zomato data,
  - Third Wave app data,
  - call-center / customer-service data,
- there was no centrally governed KPI layer,
- analytics demand was largely handled through ad-hoc requests.

---

## Approach

### 1. Discovery and Stakeholder Alignment

I started by interviewing the key business stakeholders, including the marketing, business/operations and product teams.

The goal was to understand:

- the most important decisions each team was trying to make,
- which metrics they relied on,
- where reporting or analysis was slowing those decisions down,
- and which use cases would create the highest immediate value.

### Key Business Decisions Identified

The initial analytics roadmap focused on enabling questions such as:

- Which stores were performing above or below expectations?
- What were the main drivers of store revenue?
- How were AOV, items per transaction and customer volumes changing?
- Which customer segments should marketing target?
- Which products or customer journeys required deeper product analysis?
- Which operational problems required management attention?

[VERIFY specific examples against the work you actually delivered.]

---

### 2. Data and Metric Foundation

The next step was to establish a common analytical foundation.

### Source Identification

We mapped the primary data sources required for the first analytics use cases:

- POS / store transaction data,
- Swiggy,
- Zomato,
- app/customer data,
- call-center/customer-service data.

### Metric Standardization

I worked with stakeholders to define common definitions for important business KPIs such as:

- revenue,
- AOV,
- items per transaction (IPT),
- store revenue,
- new customer,
- retention,
- ARPU,
- customer frequency.

The objective was to ensure that leadership and business teams were discussing the same numbers rather than maintaining team-specific definitions.

### Data Quality

Before scaling dashboard adoption, we introduced basic validation checks around:

- source completeness,
- reconciliation of revenue across systems,
- duplicate / missing records,
- store-level mapping,
- consistency of metric calculations.

[VERIFY which checks were explicitly implemented.]

### Ownership

For important business metrics, we clarified:

- the business definition,
- the underlying source,
- the calculation logic,
- and the owner responsible for resolving discrepancies.

This became the basis for creating a single source of truth.

---

### 3. Analytics Delivery

Because analytics capacity was limited, I deliberately avoided trying to build everything at once.

The first major deliverables were:

#### Store Scorecard

A standardized store-performance view that enabled:

- store managers,
- area managers,
- operations teams,
- and leadership

to consistently track store-level business health.

#### Central Revenue Dashboard

A consolidated leadership view of business revenue and its major drivers.

The dashboard provided leadership with one place to review business performance instead of relying on manually consolidated reports.

### Prioritization

Analytics demand was divided into:

- recurring / operational reporting,
- high-impact business analysis,
- new analytical requests,
- ad-hoc requests.

Requests were prioritized based on:

- business impact,
- urgency,
- recurrence,
- stakeholder reach,
- and analytical effort.

This also allowed us to establish clearer turnaround expectations with stakeholders.

---

### 4. Adoption and Self-Service

Building dashboards was not sufficient; adoption was treated as a separate objective.

I conducted training sessions for:

- store managers,
- area managers,
- and other business users

to explain:

- how to use the dashboards,
- how metrics were defined,
- and how to interpret the outputs.

### Self-Service

The objective was to progressively move recurring analytical questions away from manual analyst requests and into standardized dashboards / reusable views.

For marketing, the longer-term goal was to support self-service customer segmentation for campaign targeting.

[VERIFY how much of the marketing self-service capability was actually delivered during your tenure.]

### Feedback Loop

We used recurring feedback from users to improve:

- dashboard usability,
- metric definitions,
- prioritization,
- and the analytical views being delivered.

I also created a fortnightly analytics newsletter for the leadership team highlighting important business trends, observations and analytical insights.

---

### 5. Analytics Operating Model

To make the function scalable, I introduced a more structured operating model.

### Intake and Prioritization

Instead of handling every request independently, requests were categorized and prioritized based on:

- recurring vs one-time need,
- business impact,
- urgency,
- effort,
- and expected user base.

Clear turnaround expectations were communicated to functional leaders.

### Operating Cadence

We established:

- weekly analytics prioritization meetings,
- monthly business reviews,
- recurring stakeholder feedback,
- and leadership communication through the analytics newsletter.

The objective was to move analytics from reactive reporting toward a predictable business capability.

---

## Key Decision / Trade-off #1 — Standardized Metrics vs Team-Specific Definitions

### Situation

Different teams were using different definitions for important metrics such as:

- new customer,
- retention,
- ARPU.

### Options

1. Allow teams to continue using their own definitions.
2. Establish standardized company-level definitions.

### Decision

I pushed for standardized KPI definitions for the core business metrics.

### Why

Without common definitions, dashboards would create more disagreement rather than more trust.

Standardization was necessary to establish a single source of truth and allow leadership to compare performance consistently.

---

## Key Decision / Trade-off #2 — What to Build First

### Situation

Different teams wanted different analytical products:

- store scorecards,
- forecasting views,
- self-service dashboards,
- funnel analysis,
- customer analytics.

However, analytics capacity was limited.

### Decision

We prioritized two foundational products first:

1. Store Scorecard
2. Central Revenue Dashboard

### Why

These addressed the widest set of recurring business needs while allowing us to validate data quality and metric definitions before expanding the analytics layer.

The objective was to build trust and adoption before adding more sophisticated analytical products.

---

## Stakeholder Challenge

One of the biggest challenges was managing ad-hoc analytical requests.

Every business function wanted rapid turnaround, but analytics capacity was limited.

At the same time, inconsistent metric definitions meant that answering requests quickly could sometimes reinforce conflicting versions of the truth.

My approach was:

1. standardize the most important metrics first,
2. categorize requests by type,
3. introduce a prioritization framework,
4. communicate expected turnaround times,
5. move recurring questions into reusable dashboards wherever possible.

This reduced the dependency on purely reactive analytics.

---

## Results

### Leadership

Leadership gained a centralized view of business revenue and key business-health metrics.

This reduced dependence on manually consolidated reporting and created a common reference point for business reviews.

### Operations / Business

Within approximately 3–4 months, we had established a standardized store scorecard.

The scorecard was used by more than 100 store managers, area managers and other business users on a daily basis.

This became one of the core self-service analytics products for store-performance monitoring.

### Product / Marketing

The analytics function began supporting product and marketing teams with:

- customer segmentation,
- campaign / customer analysis,
- product-performance analysis,
- and experimentation measurement.

[VERIFY the exact product/marketing outputs before using this section in an interview.]

### Analytics Function

We moved the organization from:

- fragmented reporting,
- inconsistent metric definitions,
- and heavily ad-hoc analytics

toward:

- standardized business metrics,
- reusable analytical products,
- structured prioritization,
- recurring analytics operating cadence,
- and increased self-service adoption.

---

## What I Learned

### 1. Metric alignment should precede dashboard development

A technically correct dashboard is not useful if stakeholders disagree about the meaning of the metrics.

### 2. Analytics teams need explicit prioritization

Without a structured intake process, the team naturally becomes an ad-hoc reporting function.

### 3. Self-service requires governance

Giving users access to dashboards is not enough.

Self-service requires:

- trusted metrics,
- understandable definitions,
- high data quality,
- appropriate training,
- and clear ownership.

---

## What I Would Do Differently Today

### Formalize metric governance earlier

I would establish a formal metric dictionary and ownership model at the beginning rather than allowing definitions to mature organically.

### Introduce a semantic / governed metric layer earlier

Rather than embedding KPI logic independently into dashboards, I would centralize reusable business logic earlier so that downstream products consume the same definitions.

### Measure analytics adoption explicitly

I would instrument metrics such as:

- active dashboard users,
- repeat usage,
- time-to-insight,
- percentage of recurring questions handled through self-service,
- stakeholder satisfaction,
- and analytical product reuse.

This would allow the analytics team's effectiveness to be measured using business impact and adoption rather than simply the number of dashboards delivered.

## 2. 6x Pickup Revenue Growth
# Case Study 2 — Growing Store-Pickup Revenue ~6×

## Context

Third Wave customers had the option to place a store-pickup order through the mobile app.

Customers could order in advance and collect their coffee approximately 15–20 minutes later from the selected store, reducing in-store waiting time.

The business wanted to increase adoption of this behavior, partly inspired by the pickup model used by global coffee chains such as Starbucks.

---

## Baseline

At the time:

- monthly pickup revenue was approximately ₹4–5 lakh,
- pickup adoption was still relatively low,
- the feature was app-only,
- usage appeared concentrated among high-frequency, high-value customers.

I do not recall the exact pickup order count or share of total company revenue, so those numbers should not be quoted unless verified.

---

## Business Problem

The core business question was:

> Which customers were most likely to adopt pickup, and how could we increase repeat pickup behavior rather than just drive one-time trial?

The opportunity was attractive because the existing pickup users tended to be:

- high-frequency customers,
- relatively high-value customers,
- weekday-heavy users,
- and customers likely to benefit from time savings.

This made pickup potentially valuable not only as a revenue channel but also as a retention and convenience proposition for frequent customers, especially office-goers.

The desired outcome was to make ordering coffee more convenient for customers who wanted to avoid waiting in-store before work or during short breaks.

---

## Primary KPI

### Primary KPI

**Monthly pickup revenue**

### Driver Metrics

- number of pickup customers,
- orders per pickup customer,
- pickup AOV,
- repeat pickup rate,
- frequency of pickup usage.

### Guardrails

- total company revenue,
- store operational load,
- customer wait time / pickup readiness,
- excessive dependence on discounts.

---

## Analysis / Segmentation

I first analyzed customers who had used pickup during the previous 3–6 months and created a behavioral profile of existing pickup users.

The analysis showed several patterns:

- pickup customers tended to be high-frequency cafe customers,
- usage was concentrated more on weekdays than weekends,
- users were necessarily app customers because pickup was an app-only feature,
- adoption was concentrated around a smaller number of stores,
- some of the highest-usage stores were located near office clusters.

Based on these patterns, I created a rough high-propensity customer profile.

The most relevant behavioral signal was **order frequency**.

---

## Key Insight

Customers with very high purchase frequency — roughly those making more than 3–4 orders per week — appeared much more likely to use pickup.

This suggested that the best initial audience was not the entire customer base.

Instead, we should focus on highly engaged app customers who already had frequent cafe consumption behavior and were more likely to value speed and convenience.

---

## Action

I created a targeted customer segment focused on the highest-frequency app customers, approximately the top 10% by order frequency.

The campaign strategy included:

- targeted app push notifications,
- pickup-specific messaging,
- and an introductory incentive for the first few pickup orders to reduce the barrier to trial.

The broader objective was not only to generate first-time pickup orders but to establish repeat pickup behavior.

Marketing owned campaign execution and communication.

---

## My Contribution

I owned the analytics side of the initiative.

My contribution included:

- analyzing historical pickup-user behavior,
- identifying the strongest customer characteristics associated with pickup adoption,
- defining the high-propensity target segment,
- providing the customer list / segmentation logic to Marketing,
- defining the primary business metric and supporting driver metrics,
- and monitoring pickup performance after the campaign launched.

I also helped distinguish whether growth was coming from more pickup customers, higher frequency, or changes in AOV.

[VERIFY the exact extent of post-campaign monitoring.]

---

## Measurement

There was no randomized A/B test or formal control group.

Therefore, I would not claim that the campaign alone caused the full revenue increase.

The measurement approach was based primarily on:

- pre- vs post-initiative pickup revenue,
- pickup customer growth,
- repeat usage,
- and order frequency among targeted customers.

The appropriate way to describe the result is:

> Pickup revenue increased approximately 6× following the targeted initiative.

Other factors such as organic growth, new stores, seasonality, and broader app adoption could also have contributed.

---

## Result

Pickup revenue increased from approximately **₹4–5 lakh per month to roughly ₹25–30 lakh per month**, representing approximately **6× growth**.

The growth appeared to be driven primarily by:

- increased adoption among high-frequency customers,
- repeat pickup usage,
- and targeted activation of customers already showing strong purchase frequency.

An additional benefit was that pickup became a more visible and repeatable use case within the app rather than remaining a niche feature.

[VERIFY exact end-state revenue and repeat-usage figures before quoting them externally.]

---

## Key Decision / Trade-off

### Situation

We had two broad options:

1. promote pickup to the entire app customer base,
2. target customers with the highest likelihood of repeat usage.

### Decision

We chose a targeted strategy focused on the highest-frequency customers rather than a broad campaign.

### Why

A broad campaign would likely have required more discount spend and could have produced many one-time users.

The targeted approach was intended to:

- improve conversion efficiency,
- reduce unnecessary promotional spend,
- and maximize the likelihood of repeat behavior.

We also used introductory discounts only as an initial activation mechanism rather than making pickup permanently discount-led.

---

## Stakeholder Challenge

The main challenge was balancing **marketing reach** with **targeting precision**.

A broader campaign could have produced more immediate exposure, but it also risked higher promotional cost and lower-quality adoption.

My role was to use customer behavior data to make the case for focusing first on high-propensity users rather than sending the same campaign to everyone.

This required aligning Analytics and Marketing on:

- who should be targeted,
- why that segment was selected,
- and what success should look like beyond just campaign opens or clicks.

[VERIFY whether this was the actual stakeholder discussion.]

---

## What I Learned

### 1. Targeting quality matters more than audience size

High-propensity behavioral segments can outperform broad targeting when the objective is repeat behavior rather than one-time trial.

### 2. Revenue growth should be decomposed

A large increase in revenue is more useful when broken into:

- more customers,
- higher frequency,
- higher AOV,
- and stronger repeat usage.

### 3. Promotions should be evaluated beyond the promotional window

The real success metric is whether customers continue using the feature after the incentive disappears.

---

## What I Would Do Differently Today

### 1. Use a formal holdout group

I would create a control / holdout group so that we could measure incremental lift rather than relying only on pre/post comparisons.

This would allow us to estimate how much pickup growth was actually caused by the campaign.

### 2. Track post-promotion retention

I would explicitly measure:

- repeat pickup rate after 7/30/60 days,
- order frequency after the first three incentivized orders,
- and how many users continued pickup behavior without a discount.

### 3. Measure contribution margin, not only revenue

I would include:

- discount cost,
- operational cost,
- incremental margin,
- and any cannibalization from delivery or in-store purchases.

This would provide a more complete view of whether pickup growth created sustainable business value.

### 4. Build a propensity model / scoring framework later

Once enough behavioral data was available, I would move beyond simple rule-based segmentation and build a lightweight pickup-propensity score using variables such as:

- purchase frequency,
- recency,
- store proximity,
- weekday behavior,
- app engagement,
- and historical product preferences.


## 3. Recommendation System + A/B Test / AOV
# Case Study 3 — Priority-Based Recommendation Engine + A/B Test

## Context

Third Wave Coffee's app already showed product recommendations, but these were largely based on static rules.

At the time, average Items per Transaction (IPT) was approximately **1.5**, and many customers were ordering a single beverage and checking out.

This created an opportunity to improve basket size by showing more relevant cross-sell recommendations.

---

## Business Problem

The business objective was to increase:

- Items per Transaction,
- Average Order Value,
- and recommendation-driven add-ons,

without negatively affecting checkout conversion.

The existing static recommendation logic was limited because it did not sufficiently account for the customer's current basket or contextual relevance.

---

## Baseline

- IPT: approximately **1.5**
- Existing recommendation logic: static rules
- AOV: **[ADD LATER]**
- Recommendation attach rate: **[ADD LATER]**

---

## Recommendation Approach

Because time to market was important, I chose a **priority-based recommendation approach** rather than building a more complex ML recommendation system.

Candidate products were prioritized based on signals such as:

- relevance to the current basket,
- historical product affinity,
- category complementarity,
- popularity,
- store availability,
- and business rules.

[VERIFY exact production logic later.]

The objective was to ship a practical MVP quickly, validate whether more relevant recommendations created measurable business value, and only then justify investment in a more sophisticated model.

---

## Key Decision / Trade-off

### Situation

We could either:

1. build a more sophisticated ML-based recommender, or
2. ship a simpler priority-based recommendation system quickly.

### Decision

I chose the priority-based approach.

### Why

It was:

- faster to implement,
- easier to explain and debug,
- lower engineering effort,
- and sufficient to test the underlying business hypothesis.

The principle was:

> Validate incremental business value before investing in model sophistication.

---

## My Contribution

I owned the analytics / recommendation design.

My contribution included:

- identifying basket-size improvement as the opportunity,
- analyzing historical purchase behavior,
- defining recommendation priority logic,
- partnering with Product and Engineering on implementation,
- defining the A/B test measurement framework,
- and analyzing the experiment results.

---

## A/B Test Hypothesis

> Showing more relevant priority-based recommendations will increase Items per Transaction and AOV without materially reducing checkout conversion.

---

## A/B Test Design

### Control

Existing static recommendation experience.

### Treatment

New priority-based recommendation experience.

### Randomization Unit

**[ADD LATER — likely user/session/order]**

### Traffic Split

**[ADD LATER]**

### Experiment Duration

**[ADD LATER]**

### Primary Metric

**Items per Transaction**

### Secondary Metrics

- Average Order Value
- recommendation attach rate
- recommended-item add-to-cart rate
- revenue per order

### Guardrail Metrics

- checkout conversion
- cart abandonment
- order completion
- app/page latency

### Sample Size / Power

**[ADD LATER]**

---

## A/B Test Result

The treatment group showed a positive improvement versus the existing static recommendation experience.

### Result Summary

- IPT:
  - Control: **[ADD LATER]**
  - Treatment: **[ADD LATER]**
  - Uplift: **[ADD LATER]%**

- AOV:
  - Control: **[ADD LATER]**
  - Treatment: **[ADD LATER]**
  - Uplift: **[ADD LATER]%**

- Checkout conversion:
  - **[ADD LATER]**

- Statistical significance / confidence interval:
  - **[ADD LATER]**

The key result was that the recommendation approach improved basket economics while keeping the core checkout experience within acceptable guardrails.

---

## Interpretation

The experiment suggested that the improvement was driven primarily by customers adding complementary products to existing beverage orders.

The recommendation system therefore improved basket size not by changing the core purchase journey, but by increasing successful cross-sell behavior.

[VERIFY exact driver once numbers are recovered.]

---

## Business Impact

The experiment gave the business evidence that recommendation quality could be a meaningful lever for:

- improving IPT,
- improving AOV,
- and increasing incremental order value.

It also justified further investment in more sophisticated recommendation and personalization capabilities.

Exact annualized or monthly business impact:

**[ADD LATER]**

---

## Stakeholder Challenge

The main trade-off was between speed to market and technical sophistication.

Rather than delaying delivery to build a complex recommender, I aligned Product and Engineering around a simpler testable MVP.

The A/B test allowed us to make the next investment decision using evidence rather than assuming that greater model complexity would automatically create more value.

---

## What I Learned

1. **Experimentation is more important than model sophistication.**
   A simpler model with a well-designed A/B test can create more business confidence than a sophisticated model without causal evidence.

2. **Recommendation success should be measured using business metrics.**
   Click-through rate is useful, but IPT, AOV, attach rate and conversion matter more.

3. **Guardrails are essential.**
   AOV growth is not useful if the recommendation experience damages checkout conversion.

---

## What I Would Do Differently Today

I would strengthen the experiment by explicitly defining upfront:

- Minimum Detectable Effect,
- statistical power,
- sample-size requirements,
- experiment duration,
- and segmentation of results.

I would also analyze heterogeneous treatment effects across:

- high-frequency vs low-frequency customers,
- store type,
- product category,
- time of day,
- and new vs repeat customers.

If the MVP continued to show incremental value, I would then evolve the solution toward more personalized ranking using customer-level behavioral signals.


## 4. Medallion / Data Platform

## 5. Amazon FADS +700 bps

## 6. AiDash Analytics / Data / AI Implementation
