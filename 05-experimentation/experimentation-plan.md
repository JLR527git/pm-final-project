# A/B Experiment Brief, RouteLogic (B2B)

## Parameters
| Parameter | Decision |
|---|---|
| Feature under test | One-Click Compliance Checklist The largest predicted benefit to compliance and reporting time |
| Persona | Dispatch Coordinators |
| Expected outcome | Faster route reporting |
| Primary success metric | Compliance check completion rate |
| Baseline rate | 48 |
| Guardrail metric | Usage of live dispatch tool |
| Guardrail boundary | 5% drop |
| Second guardrail | · |
| Minimum Detectable Effect | 10 |
| Sample size per arm | 390 |
| Traffic split | 50/50 |
| Test duration | 2 months |
| Significance threshold | p < 0.05 |

## Control vs. Variant
- **Control (A):** The current RouteLogic flow
- **Variant (B):** The one screen streamlined compliance reporting
- **Held constant (isolation check):** Onboarding
Route management

## Hypothesis
> I believe that One-Click Compliance Checklist The largest predicted benefit to compliance and reporting time for Dispatch Coordinators will result in Faster route reporting, as measured by a 10 change in Compliance check completion rate within 2 months. We will protect Usage of live dispatch tool throughout the test.

## Shipping criteria
> We will **ship** if Compliance check completion rate improves by ≥ 10 at p < 0.05 and Usage of live dispatch tool does not reach 5% drop after 2 months.
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of 2 months, no results reviewed before this date.
