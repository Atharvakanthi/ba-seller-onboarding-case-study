# KPI Framework

This framework defines the metrics used to evaluate the fictional PropCo seller/developer onboarding redesign. Each KPI ties directly back to an objective in the [BRD](BRD.md).

| KPI | Definition | Why it matters |
|---|---|---|
| **Onboarding completion rate** | % of started seller/developer onboarding forms that reach final submission. | Directly measures whether the redesigned form reduces abandonment versus the fragmented as-is forms. A low rate signals friction, confusing fields, or excessive length. |
| **Time-to-list** | Elapsed time from first seller/developer contact to the profile/listing going live on the buyer platform. | Captures the end-to-end effect of removing manual re-keying and clarification email loops. This is the metric the Head of Sales cares about most, since it reflects advisor and seller experience together. |
| **Data-field completeness / accuracy** | % of required fields populated with values conforming to the shared variable dictionary's allowed value sets, at first submission. | Directly reflects whether the standardized variable dictionary and inline validation are working. Low completeness upstream is the root cause of both re-keying effort and poor recommendation matches. |
| **Seller/developer drop-off rate (by form step)** | % of sellers/developers who start but abandon the form, broken out by the specific step where they stop. | Pinpoints exactly which section of the form causes friction, so future iterations target the right fields rather than redesigning the whole form blindly. |
| **Onboarding Ops manual-intervention rate** | % of submissions that require Ops to contact the advisor/seller for clarification or manual correction. | Measures whether the redesign actually reduces operational rework, which was one of the original pain points driving this project. |
| **Recommendation-match accuracy** | % of buyer-facing recommendations generated from a seller/developer profile that are rated as relevant matches (via existing buyer feedback/acceptance signals). | Connects onboarding data quality to the ultimate business outcome — better matches drive better buyer engagement and, ultimately, more successful transactions. |
| **Time-per-submission for Ops review** | Average Ops handling time per submission, from receipt to publish. | Quantifies operational efficiency gains from reduced manual re-keying, supporting a capacity/cost argument for the redesign. |
| **Regional consistency variance** | Standard deviation of completion rate and time-to-list across the three regions. | A successful unification should shrink regional variance close to zero; persistent variance signals the unified form isn't actually being used uniformly. |

## Baseline & target approach

For each KPI, this case study recommends:
1. Capturing an **as-is baseline** over a fixed observation window before rollout (e.g., the prior full quarter).
2. Rolling out the redesigned form to a pilot region first, comparing pilot metrics against the baseline and against the two non-pilot regions.
3. Expanding to all regions only once the pilot shows improvement on completion rate, time-to-list, and data-field completeness without a corresponding negative shift in drop-off rate.

## Reporting cadence

- **Weekly:** completion rate, drop-off rate by step, Ops manual-intervention rate (operational, fast-feedback metrics).
- **Monthly:** time-to-list, time-per-submission, regional consistency variance (trend metrics, less noisy at monthly granularity).
- **Quarterly:** recommendation-match accuracy (requires enough downstream buyer interaction volume to be statistically meaningful).
