# Business Requirements Document (BRD)

**Project:** Seller & Developer Onboarding Redesign
**Client (fictional):** PropCo — a fictional proptech company used solely as a teaching example for this case study
**Document owner:** Business Analyst (case study author)
**Status:** Demonstration artifact — not a real client engagement

> **Note on this document:** PropCo, its people, its forms, and all data referenced below are entirely fictional. This BRD was written to demonstrate business analysis method (requirements gathering, process mapping, and recommendation writing) for a Data/Business Analyst portfolio. No real company, client, or individual is represented.

---

## 1. Problem Statement

PropCo is a real-estate marketplace that connects property **sellers** and **developers** with buyers through a network of sales advisors and an online listings platform. Over the past two years, PropCo's seller/developer intake process grew organically across three regional teams, each of which built its own intake spreadsheet and its own version of a "developer profile" form.

This produced three compounding problems:

1. **Inconsistent data capture.** The same concept (e.g., "possession date," "project stage," "price band") is captured under different field names, different formats, and sometimes not at all, depending on which regional team onboarded the seller.
2. **Broken downstream recommendations.** PropCo's buyer-matching engine relies on structured seller/developer attributes to recommend listings to prospective buyers. Inconsistent or missing fields degrade match quality, which sales advisors have flagged as a recurring complaint.
3. **Slow, error-prone onboarding.** Sellers and developers report that onboarding forms feel repetitive and unclear, leading to incomplete submissions, back-and-forth clarification emails, and a multi-week delay between first contact and a listing going live.

PropCo's leadership has asked for a business analysis engagement to diagnose the root causes and recommend a redesigned onboarding process and intake form structure.

---

## 2. Stakeholders

| Stakeholder | Role in this initiative |
|---|---|
| **Head of Sales** | Business sponsor. Owns the sales advisor teams who run onboarding conversations with sellers/developers. Primary success measure: faster time-to-list and fewer advisor escalations. |
| **Product Manager, Buyer Platform** | Owns the buyer-facing listings and recommendation engine. Needs consistent, structured seller/developer data to keep match quality high. |
| **Onboarding Ops Lead** | Manages the operations team that manually reviews and cleans intake submissions before they reach the platform. Closest to the day-to-day pain of inconsistent data. |
| **Regional Sales Advisors (3 regions)** | Front-line users who fill in or help sellers fill in the intake form. Represent the three divergent regional practices this project must reconcile. |
| **Sellers / Developers** | External users submitting property and project information. Their experience of the form directly affects completion and drop-off rates. |
| **Data & Analytics Lead** | Owns reporting on onboarding funnel metrics and recommendation-engine performance; consumer of the KPIs defined in this project. |
| **Business Analyst (case study author)** | Facilitates requirements gathering, process mapping, and produces the recommendation. |

---

## 3. Objectives

1. Standardize seller/developer intake data capture into a single, shared field taxonomy used across all three regions.
2. Redesign the intake and developer-profile forms to reduce redundant questions and clarify ambiguous fields (e.g., ensure every variable has one agreed definition, used consistently across all forms).
3. Reduce seller/developer onboarding time-to-list and reduce the rate of incomplete submissions requiring manual follow-up.
4. Improve the structured-data inputs available to the buyer recommendation engine, to raise recommendation-match accuracy.
5. Produce a repeatable process (as-is → to-be) that Onboarding Ops can maintain without ad hoc regional variation.

---

## 4. Scope

**In scope:**
- Requirements gathering with Sales, Product, Onboarding Ops, and a sample of sellers/developers (represented here as fictional personas/interviews).
- As-is process mapping of the current seller/developer onboarding journey across the three regions.
- To-be process design for a unified onboarding journey.
- A consolidated field taxonomy / variable dictionary reconciling the three regional forms.
- User stories describing the redesigned onboarding and profile-intake experience.
- A KPI framework to measure the redesign's impact.

**Out of scope:**
- Actual engineering build of the new form or platform changes (this case study produces requirements and recommendations, not production code).
- Pricing, commercial, or contractual terms between PropCo and sellers/developers.
- Buyer-side onboarding or buyer app redesign.
- Marketing or lead-generation process changes upstream of first seller/developer contact.
- Any real production data, systems, or named organizations — all data and artifacts in this repository are fictional.

---

## 5. Assumptions & Constraints

- PropCo's three regional teams will continue operating independently for other purposes; this project only unifies the onboarding data model and process, not full regional org structure.
- The redesigned form must be completable by a non-technical seller or developer without advisor assistance, but should also support an advisor filling it in on the seller's behalf during a call.
- Any variable used in the recommendation engine must have a single, unambiguous definition documented in the variable dictionary before the form is finalized.
