# User Stories

All stories below describe the fictional PropCo seller/developer onboarding redesign. Roles are invented personas for this case study.

---

### 1. Unified intake form
**As a** Regional Sales Advisor,
**I want** a single onboarding form that works the same way in every region,
**so that** I no longer need to remember which regional spreadsheet to use or reconcile field differences later.

Acceptance criteria:
- One form definition is used across all three regions with no region-specific field variants.
- Advisor can complete the form for a seller during a live call without switching tools.
- Form is accessible from the same entry point regardless of region.

---

### 2. Inline field validation
**As a** Seller,
**I want** the onboarding form to tell me immediately if a field is missing or invalid,
**so that** I don't submit an incomplete profile and wait days for someone to email me about it.

Acceptance criteria:
- Required fields are marked clearly before submission.
- Invalid entries (e.g., a non-numeric price) are flagged inline with a plain-language message.
- Submission is blocked only for required fields; optional fields never block submission.

---

### 3. Shared variable dictionary
**As an** Onboarding Ops Lead,
**I want** every field on the intake form to map to one agreed definition in a shared variable dictionary,
**so that** I stop having to guess what a regional team meant by a given field before re-keying it.

Acceptance criteria:
- A variable dictionary document exists listing every field, its definition, data type, and allowed values.
- Every field on the unified form references exactly one entry in the dictionary.
- No two fields in the dictionary share overlapping or ambiguous definitions.

---

### 4. Developer profile redesign
**As a** Developer (property developer persona),
**I want** a profile form that only asks project-level questions relevant to my project type,
**so that** I don't answer irrelevant questions meant for individual sellers.

Acceptance criteria:
- Form branches based on submitter type (individual seller vs. developer/project).
- Developer branch surfaces project-level fields (e.g., project stage, unit mix, possession timeline).
- Individual-seller branch hides project-level fields entirely.

---

### 5. Reduced re-keying by Ops
**As an** Onboarding Ops Lead,
**I want** validated submissions to route directly into the shared system without manual re-entry,
**so that** my team can spend time on genuine edge cases instead of routine data transcription.

Acceptance criteria:
- Submissions that pass validation flow into the shared system automatically.
- Ops dashboard shows only submissions flagged for review, not the full volume.
- Time spent per submission by Ops is measurably reduced versus the as-is process.

---

### 6. In-form clarification instead of email threads
**As a** Regional Sales Advisor,
**I want** to resolve a flagged field directly inside the form/system,
**so that** I don't have to dig through email threads to find what Ops is asking about.

Acceptance criteria:
- Flagged fields carry a visible comment/note from Ops.
- Advisor or seller can respond and resubmit within the same record.
- A history of clarification requests is retained on the record.

---

### 7. Consistent recommendation-ready fields
**As a** Product Manager for the Buyer Platform,
**I want** seller/developer profiles to always populate the structured fields the recommendation engine depends on,
**so that** buyer-facing matches stay accurate regardless of which region or advisor onboarded the seller.

Acceptance criteria:
- Recommendation-critical fields are marked "required" on the unified form.
- No profile can be published to the buyer platform with a recommendation-critical field empty.
- Field values conform to the shared variable dictionary's allowed value sets.

---

### 8. Onboarding funnel visibility
**As a** Data & Analytics Lead,
**I want** a dashboard tracking onboarding completion rate, time-to-list, and drop-off point,
**so that** I can tell leadership whether the redesign is working and where sellers still struggle.

Acceptance criteria:
- Dashboard shows completion rate and average time-to-list, updated regularly.
- Dashboard identifies the specific form step where most drop-offs occur.
- Metrics are comparable to a documented as-is baseline.

---

### 9. Self-serve seller onboarding
**As a** Seller,
**I want** to be able to start and save my onboarding form without an advisor present,
**so that** I can complete it on my own schedule instead of only during a live call.

Acceptance criteria:
- Form supports save-and-resume without data loss.
- Seller receives a confirmation once the form is fully submitted.
- Advisor can still open and assist with an in-progress submission if requested.

---

### 10. Regional exception handling
**As an** Onboarding Ops Lead,
**I want** a documented process for the rare cases where a region has a genuinely unique legal or regulatory field requirement,
**so that** unifying the form doesn't force us to silently drop a field a region actually needs.

Acceptance criteria:
- An exception-request process exists for adding a region-specific field.
- Any approved exception is added to the shared variable dictionary with its scope noted.
- Exceptions are reviewed periodically rather than accumulating unmanaged.

---

### 11. Head of Sales visibility into advisor workload
**As the** Head of Sales,
**I want** to see how onboarding time-to-list changes after the redesign,
**so that** I can report the impact to leadership and decide whether to extend the approach to other workflows.

Acceptance criteria:
- Time-to-list is tracked before and after redesign rollout.
- Report breaks out time-to-list by region to confirm consistency.
- Report is available without requesting a custom pull from Data & Analytics.

---

### 12. Recommendation-match accuracy tracking
**As a** Product Manager for the Buyer Platform,
**I want** to measure recommendation-match accuracy before and after the onboarding redesign,
**so that** I can attribute any improvement in buyer match quality to better upstream seller/developer data.

Acceptance criteria:
- A baseline recommendation-match accuracy metric is captured pre-redesign.
- The same metric is tracked post-redesign on a comparable cohort.
- Metric definition is documented so it can be recomputed consistently over time.
