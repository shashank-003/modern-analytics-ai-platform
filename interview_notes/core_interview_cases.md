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

## 3. Recommendation System + A/B Test / AOV

## 4. Medallion / Data Platform

## 5. Amazon FADS +700 bps

## 6. AiDash Analytics / Data / AI Implementation
