# TASK 1 — Daily Clinic Inventory Micro-Audit System

## Objective
Set up a lightweight daily control routine that detects small inventory and billing errors early, keeps staff attentive, and prevents month-end stock surprises without consuming doctor time.

---

## Daily Checklist (20–25 minutes)
- Name variation check for high-risk medicines
- Stock usage reasonableness check
- Random bill spot check
- Error logging

---

## Weekly Checklist (15 minutes)
- Review error patterns
- Decide retraining or SOP updates
- Escalate only if escalation rules are met

---

## Step 1 — Identify High-Risk Medicines
Criteria used:
- High daily usage
- Similar or confusing names
- Frequently prescribed medicines

| Medicine (Master Name) | Reason |
|------------------------|--------|
| Dolo 650 | High volume and many name variations |
| Azithromycin 500 | Frequently abbreviated |
| Pantoprazole 40 | High OPD frequency |

---

## Step 2 — Daily Name-Variation Check
Sales entries are filtered to high-risk medicines and grouped manually using a simple name-mapping list.

| Entered Name Variants | Standard Name |
|----------------------|---------------|
| Dolo / Dolo kind / Dolo 650 | Dolo 650 |
| Azithro / Azithromycin | Azithromycin 500 |

New or confusing variants are added to the mapping list and billing staff are informed the same day.

---

## Step 3 — Daily Usage Reasonableness Check
Expected Closing Stock = Opening + Purchases − Sales (after grouping)

| Medicine | Expected | Actual | Difference | Action |
|----------|----------|--------|------------|--------|
| Dolo 650 | 1460 | 1440 | −20 | Review entries |

Variance beyond ±2% triggers review.

---

## Step 4 — Random Bill Spot Check
3–5 random bills involving high-risk medicines are checked daily to verify correct names and reasonable quantities.

Errors are corrected and logged without penalties.

---

## Step 5 — Pattern Tracking
A weekly error log is maintained.

| Date | Medicine | Error Type | Repeated |
|------|----------|------------|----------|
| Aug 1 | Dolo 650 | Name variation | Yes |
| Aug 3 | Dolo 650 | Quantity error | No |

Repeated errors lead to retraining or SOP clarification.

---

## Step 6 — Doctor Escalation Rules
Doctor involvement is required only if:
- Financial impact is significant
- Errors persist despite correction
- Inventory issues affect patient treatment
