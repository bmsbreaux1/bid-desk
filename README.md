# bid-desk

An AI bid desk for offshore marine construction: RFQ in, lump-sum proposal out.

One agent runs the whole bid. It reads the client package, models the scope and schedule, prices ranked spread options, drafts vendor RFQs, runs the estimate sheet and cuts a versioned proposal PDF.

> This repo is a showcase. Bid numbers, vendor rates and client documents are private.

## Pipeline

1. **Intake.** Read the RFQ / RFP package and bulletins.
2. **Scope model.** Break the campaign into lines, durations and a schedule.
3. **Spread options.** Price ranked vessel and equipment spreads (A to D), cheapest first.
4. **Vendor RFQs.** Draft them as Gmail drafts. A human sends.
5. **Estimate.** Run the estimate in a Google Sheet.
6. **Proposal.** Cut a versioned PDF: bid form, extra-work rates, qualifications and exhibits. Every regeneration is a new version.

## Campaign types

Pipeline flush and abandonment (PLA), pipeline removal, crossing remediation, P&A / decom support, riser and SSTI work.

## First run

A multi-line pipeline abandonment bid in the Gulf of America, October 2026, bid as an independent prime.

## Built with

Claude Code (`/bid-job` skill), Google Sheets and Gmail APIs, Python, a written bid playbook.

## Contact

Britt Breaux · britt@breauxoffshore.com · Houston, TX
