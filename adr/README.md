# Architecture Decision Records

This directory contains Architecture Decision Records (ADR) for the
Prompt-Payments project. Each ADR records the definition and formal acceptance
of any _architecturally significant_ design decisions.

> This approach helps us track the motivation behind certain decisions. It
> means we can review _why_ things were done in a particular way, and if
> we choose to supersede or deprecate a decision, it can be done in an
> informed manner.

This approach is inspired by
[Michael Nygard's article](http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions).

## How to use this directory
Each ADR exists as a standalone `markdown` document in this directory and an index
of all ADRs (and their status) is maintained in the [Index section](#index)
of this `README`. Please follow [the ADR approval workflow](#adr-workflow) below
when adding new decisions to the record.

## Index
* 001 ✅ - [Use ADRs](adr-001-use-adrs.md)
* 002 💡 - TBD
---

## ADR Workflow
Each ADR goes through the following workflow: `proposed > approved`. Use the PR
mechanism to get a decision approved. Other states include `rejected`,
`deprecated` or `superseded` (see below).

### Proposal
1. Create a new ADR document in this folder using the [ADR template](template.md).
   Use the next available index number and set status to `proposed`.
2. Update [the index](#index) with the relevant state icon.
3. Create a pull request, add appropriate reviewers (e.g. dev team, any stakeholders).

### Approval
1. Colleagues may suggest edits, comments, request clarifications or
   additional information. Update ADR file as required.
2. Once the PR is approved set the ADR status to `approved` in the ADR file
   **and** in [the index](#index).
3. Merge the PR.

### Rejection
Should the ADR be rejected, it's almost always a good idea to update and merge
the PR accordingly. This helps us to stop revisiting the same decisions
repeatedly.

### Deprecating or superseding old decisions 
ADRs (once approved or rejected) should be considered immutable. However,
sometimes a decision might be revisited, and a different conclusion is
reached. In these circumstances a new ADR should be created documenting the
context and rationale for the change in thinking.

In these circumstances a new ADR should reference the old one(s). Superseded
or deprecated ADRs should be updated and included as part of the review process.

### State Icons

- `proposed`: 💡
- `approved`: ✅
- `rejected`: ❌
- `deprecated`: ☠️
- `superseded`: 🕑

### Images
A picture paints a thousand words! Use images (preferably PNG) wherever
possible in your ADRs to help explain the proposal. Images should be kept in
the [adr/img](img) directory.
