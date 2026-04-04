# CEM501 — Week 6 Assignment: Daily Construction Report
**Spring 2026 | Dr. Eyuphan Koc | Bogazici University**

---

## Assignment: Write a Daily Report from Raw Field Notes

**Due:** April 11, 2026 (before class)

---

### Scenario

You are the assistant PM on the **Kadikoy Bridge Rehabilitation Project** (Contract #BR-2024-071). At the end of the day on March 14, 2026, you receive field notes from multiple people on site:

| File | Source | Format |
|------|--------|--------|
| `01_superintendent_morning.txt` | T. Aksoy (Superintendent) | Voice memo transcription |
| `02_hasan_beton_plus.txt` | Hasan Eren (Foreman, Beton Plus) | WhatsApp message |
| `03_mehmet_kaya_steel.txt` | Mehmet Yildiz (Foreman, Kaya Steel) | Handwritten note |
| `04_elif_project_engineer.txt` | Elif Sahin (Project Engineer) | Email |
| `05_safety_log_entry.txt` | T. Aksoy (acting Safety Officer) | Safety log page |
| `06_photo_log.txt` | Various | Photo log sheet |

These files are in the course repository at `Week06_Reports_Summarization/field_notes/`.

---

### Your Task

Consolidate all of these into a single, professional **Daily Construction Report** following the format and guidelines from the Week 6 lecture (Part II).

Use the example report in Section 2.2 of the lecture as your template. Your report must include all seven required elements:

1. **Date, project name, report number**
2. **Weather** (morning + afternoon)
3. **Manpower** (by trade, subcontractor, count)
4. **Equipment** (status: active, idle, standby)
5. **Work performed** (locations, quantities, %)
6. **Delays, issues, RFI status**
7. **Safety and visitors**

---

### Self-Check Before Submitting

- [ ] Specific locations (grid lines, spans, stations)?
- [ ] Quantities included (m3, linear meters, count)?
- [ ] Subcontractors named with crew sizes?
- [ ] Could this report support a delay claim in arbitration?
- [ ] Safety section complete — including the near-miss?
- [ ] Tone objective and factual — no editorializing?
- [ ] RFI aging and equipment idle days tracked?
- [ ] Overlapping information from multiple sources consolidated without duplication?

---

### Grading

**Grade:** Pass / Needs Revision

A passing report:
- Contains all seven required elements
- Uses specific locations, quantities, and named parties
- Records the near-miss with corrective action taken
- Tracks RFI-018 aging (days outstanding) and backhoe idle time (days idle)
- Is written in an objective, factual tone suitable for a business record
- Could be presented as evidence in a construction dispute

---

### Submission

Submit as PDF or Markdown to the course repository under `hw/week06/`.

---

## Milestone: M3 — Daily Digest Generator

**Due:** Before Week 8

**Deliverable:** `project/digest.py` pushed to your course repository

**Build steps** (use Claude Code, Codex CLI, or Gemini CLI):

| Step | Goal |
|------|------|
| 1 | Basic digest with hardcoded sample emails — runs and prints |
| 2 | Add LLM summarization for URGENT and ACTION items |
| 3 | Connect to `reader.py` and run with live inbox data |
| 4 | Customize formatting, categories, summary length |

**Stretch goal:** Add a `--format html` flag for an emailable digest.

**Requirements for digest.py:**

1. Accepts a list of email dictionaries (or reads from `reader.py`)
2. Groups emails by triage category (URGENT, ACTION, FYI, ARCHIVE)
3. Generates a one-sentence LLM summary for URGENT and ACTION items
4. Outputs a formatted text digest with date/time header
5. Works end-to-end: `python digest.py` prints a digest from your inbox
6. Includes at least 3 hardcoded test emails so the grader can verify without inbox access

**Grading:** Pass / Needs Revision

**Pass criteria:** Code runs without errors, produces a readable digest, and summaries are coherent. You do not need to handle edge cases perfectly — the goal is a working prototype.

---
**Dr. Eyuphan Koc** | eyuphan.koc@bogazici.edu.tr
