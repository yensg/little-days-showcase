# Engineering and validation

## Stack

- TypeScript, React and Next.js for the application.
- SQLite and a typed data-access layer for persistence.
- Server-side authentication, authorization and input validation.
- Background processing for operational work and optional reminders.
- Unit/integration testing and browser-based journey checks.

These describe the private application's architecture. This repository does not include its implementation or deployment configuration.

## Evidence at different levels

| Check | What it can establish | What it does not establish |
|---|---|---|
| Unit and integration tests | Specific logic and component interactions under test | Every real device or production condition |
| Browser journey checks | Selected flows and layouts in a controlled environment | Physical-phone acceptance unless actually tested |
| CI build and security checks | Buildability and the checks explicitly executed | Successful deployment or absence of every vulnerability |
| Runtime verification | Observed public access and expected running version at a point in time | Permanent availability |
| User feedback | Experience reported in real use | A universal result across all users |

## Lessons that shape the work

1. Test a thin complete journey early: opening a form is not the same as saving and reloading a record.
2. Use realistic UI states, including long text, empty lists, errors and expanded controls.
3. Separate immutable application files from explicitly permitted runtime-generated cache files.
4. Preserve useful failure evidence; a generic error can hide the distinction between failed deployment and successful startup followed by a failed check.
5. Distinguish local app health, private network access, public DNS and public HTTPS. A connected network client alone does not prove internet reachability.
6. Verify that an improvement reaches the executing workflow, not only a document or unused template.

## Continuous improvement

Feedback → classify the problem → define success → reproduce or measure → make a scoped change → review and verify → release → observe.

Preference changes, implementation defects and infrastructure failures are different categories. Each requires evidence appropriate to its cause. A successful experiment should not silently become a universal rule.

## Current boundaries

This is not a claim of medical certification, legal compliance, global-scale capacity or guaranteed alert delivery. Broader commercial operation requires additional product, security, reliability, privacy and operational work.
