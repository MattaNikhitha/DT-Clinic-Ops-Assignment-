# TASK 2 — Patient Care & Communication Control System

## Objective
Reduce doctor’s non-clinical workload by structuring patient communication and follow-ups into a controlled, review-based system.

---

## Step 1 — Message Type Classification

| Message Type | Example | Doctor Input Needed |
|--------------|---------|---------------------|
| Follow-up Reminder | Please visit on Aug 5 | No |
| Post-Procedure Care | Mild swelling is normal | No |
| Side-Effect Advisory | Nausea may occur | No |
| Custom Instruction | Avoid sun exposure for 7 days | Yes |
| Patient Question | Is itching normal? | Yes |

---

## Step 2 — Care Control Sheet
A Google Sheet (`Care_Control`) is used to track all patient communication.

| Patient | Phone | Visit Type | Message Type | Message Text | Doctor Approval | Status |
|---------|-------|------------|--------------|--------------|----------------|--------|
| Ramesh K | 9XXX | OPD | Follow-up | Auto | Not Required | Pending |
| Sita P | 9XXX | Procedure | Post-Procedure | Auto | Not Required | Pending |
| Arjun M | 9XXX | OPD | Custom | Blank | Required | Waiting |

---

## Step 3 — Doctor Review Window
Every 3–4 hours, items requiring doctor approval are reviewed in a 10-minute window. The doctor dictates once; staff records and updates.

---

## Step 4 — Patient Question Handling
Patients submit questions via Google Form. Responses are batched and reviewed with the doctor.

| Patient | Question | Answer | Status |
|---------|----------|--------|--------|
| Lakshmi | Is itching normal? | — | Pending |

---

## Step 5 — Message Dispatch Rules
Messages are sent only when:
- Message text is filled
- Status is Pending
- Doctor approval is not required or approved

Status flow: Pending → Sent → Closed

---

## Step 6 — Daily Closing Check
Before clinic closes, pending items are reviewed to ensure nothing critical is missed.

---

## Optional — Automation Logic
Pending messages can be sent automatically using Google Apps Script and WhatsApp API, with status updated after sending.
