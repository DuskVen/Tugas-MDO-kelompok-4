# Jobdesk Analysis: Clinic Registration and Initial Anamnesis

## Case description
Internship at a general clinic, supporting the registration desk and the collection of initial patient-reported information before a doctor consultation.


## Task mapping
| Work activity | Repetitive steps | Candidate agent support | Human responsibility |
|---|---|---|---|
| Registration | Ask and record required demographic/administrative fields | Conversational collection and draft record | Verify identity and authorize registration |
| Completeness review | Check if required fields are missing | Checklist and follow-up prompts | Resolve exceptions and approve record |
| Initial complaint intake | Ask complaint, duration, location, associated symptoms | Structured, progressive questioning | Clinical assessment and triage |
| Background intake | Ask approved allergy, medicine, and relevant history questions | Capture answers and mark unknowns | Confirm relevance and review |
| Summary preparation | Reformat notes for doctor | Structured draft summary | Review, correct, and use in consultation |
| Frequently asked admin information | Repeat clinic-approved instructions | Answer FAQ using clinic-provided information | Update policy, answer exceptions |

## Selected agent
**Clinic Intake Assistant** — helps collect registration details and initial patient-reported information, checks for missing fields, and drafts a handoff summary.

## Why this was selected
These steps use a relatively repeatable question-and-record pattern. AI may reduce repetitive typing and improve consistency of draft notes, but staff must remain responsible for verification, patient privacy, and clinical decisions.

## Out of scope
- Diagnosing disease or interpreting clinical symptoms
- Prescribing or recommending medication/treatment
- Clinical triage or deciding that a patient is safe to wait
- Creating or modifying records in a real clinic system
- Processing real patient records in this public demo
