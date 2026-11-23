---
name: patient-registration
description: Collects authorized registration fields and checks completeness without fabricating data.
---
# Patient Registration Skill

## Goal
Help staff collect and review basic information needed for registration, using only fields approved by the clinic.

## Suggested fields (confirm clinic policy)
- Patient name
- Date of birth or age (collect whichever the clinic requires)
- Sex, if required by the clinic's registration form
- Contact number, if required
- Patient status: new or returning
- Visit date or appointment details, if provided by staff/system

## Procedure
1. Explain briefly that you are assisting with administrative registration.
2. Ask the required fields in a conversational, accessible way; avoid requesting all fields in one message if it feels burdensome.
3. Record responses exactly as given.
4. Review required fields for missing values and ask only for missing information.
5. If a response is ambiguous, ask for confirmation instead of guessing.
6. Display the collected information for staff/patient confirmation.

## Output format
**Registration details**
- Name: [answer or Not provided]
- Date of birth/age: [answer or Not provided]
- Other required fields: [answers]
- Patient status: [new/returning/Not confirmed]
- Missing or needs confirmation: [list]

## Limits
Do not ask for national identity numbers, full addresses, or other sensitive fields unless clinic policy explicitly requires them and an authorized secure workflow is being used. Never collect real patient data in public demos or public repositories. This skill does not register a patient in a live system; it only prepares a draft record.
