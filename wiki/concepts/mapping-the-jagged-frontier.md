---
title: "Mapping the Jagged Frontier — A Profession-by-Profession Approach"
date: 2026-05-19
tags: [ai, productivity, work, llm, learning, skill-development]
related: [[jagged-frontier]], [[living-and-working-with-ai]], [[ethan-mollick]], [[cognitive-atrophy-and-ai]], [[large-language-models]]
connections:
  - type: application-of
    target: jagged-frontier
---

# Mapping the Jagged Frontier — A Profession-by-Profession Approach

How workers in any given profession should invest mapping effort to locate the [[jagged-frontier|jagged frontier]] of AI capability across the tasks that actually compose their work — and what the [[ethan-mollick|Mollick]] research suggests about who reaps the gains.

## Why Mapping Is a Personal Project

[[living-and-working-with-ai]] establishes the structural feature that makes mapping necessary: the frontier is **irregular and invisible**. Tasks that look similar in difficulty can be on opposite sides; the only way to find out is to experiment. The implication Mollick stresses repeatedly: **the world's leading expert on AI for your specific role is going to be you**, because no research team has your task inventory and no general benchmark captures the friction points of your day.

Mapping cannot be outsourced to industry reports or vendor demos. Industry-level studies (Felten, Raj, and Seamans found AI overlap with 980 of 1,016 occupations — see [[living-and-working-with-ai]]) tell you that your job overlaps; they do not tell you which 11 of your 40 weekly tasks the overlap actually lands on.

## The Mapping Method

A practical mapping protocol, derived from Mollick's "invite AI to everything" principle:

1. **Inventory tasks at a fine enough grain.** "Writing" is too coarse. Break into: drafting cold emails, summarizing meeting notes, generating outlines, copy-editing, writing technical explanations of code, writing performance reviews, writing client-facing memos. Each of these sits in a different place on the frontier.
2. **Try each task with AI three times.** Mollick's note that consultants in the BCG study were "simply pasting in the questions" describes the failure mode of insufficient mapping. One try doesn't reveal whether a task is inside, outside, or on the edge of the frontier; three tries with different prompts establishes a rough probability.
3. **Score on two axes.** Capability (did the AI produce something useful?) and **confidence-calibration** (did it admit when it didn't know, or did it confabulate?). The Dell'Acqua "falling asleep at the wheel" study (181 recruiters evaluating 44 resumes) shows that confident wrong answers from AI are the dangerous case — they corrupt human judgment more than visible failures.
4. **Mark the edges.** The most valuable knowledge is not "AI is good at X" but "AI is good at X except when X involves Y" — counting words, exact arithmetic, recent events, citations, applying domain-specific rules. These exceptions are where the frontier turns.
5. **Re-run quarterly.** Capability improves; the frontier moves. Mollick's fourth rule — "assume this is the worst AI you'll ever use" — is mapping advice as well as adoption advice. Cached mental maps go stale within months.

## Where the Frontier Currently Falls — By Profession

The patterns below summarize what *Co-Intelligence* and the wiki's existing [[cognitive-atrophy-and-ai]] page identify; in every case the personal mapping is what matters, not the table.

### Software development
- **Inside (high capability):** boilerplate, regex, type-safety refactors, translating between languages, drafting tests for known interfaces, explaining unfamiliar code, generating standard React/SQL/API patterns.
- **Edge:** complex debugging, architecture decisions with conflicting constraints, performance tuning that requires runtime measurement.
- **Outside:** anything requiring true reasoning about state across long codebases, security-sensitive correctness, novel algorithm design.

### Clinical medicine
- **Inside:** literature summary, differential diagnosis brainstorming, patient-facing explanation of known conditions, note dictation cleanup, ICD coding assistance.
- **Edge:** triage on ambiguous presentations, weighing competing guidelines.
- **Outside:** physical exam interpretation, the implicit communication of patient cues, decisions where the cost of confident error is catastrophic.

### Law
- **Inside:** first-pass document summarization, clause comparison, drafting standard contract language, explaining doctrine to a client.
- **Edge:** issue-spotting in novel facts.
- **Outside:** citations (LLMs fabricate cases — the Mata v. Avianca pattern), jurisdiction-specific rule application, strategic judgment about what to argue.

### Management consulting (Mollick's BCG-studied population)
- **Inside:** the 18 BCG tasks — idea generation, market segmentation, draft press releases, internal memos. Consultants using AI were faster, judged more creative, better written, and more analytical.
- **Outside:** the one BCG task designed with "a tricky statistical issue and misleading data" — unaided consultants got it right 84% of the time; AI-aided consultants got it right only 60–70%, because the AI gave a confident wrong answer they did not catch.

### Teaching
- **Inside:** lesson plan drafts, differentiated explanation of a concept at multiple levels, generating practice problems, feedback on student drafts.
- **Edge:** formative assessment design, calibrating challenge to a specific student.
- **Outside:** the relational/motivational work that drives engagement (the question from [[ai-tutoring]] about whether AI tutoring replicates the motivational component).

### Writing / journalism
- **Inside:** research summarization, outline generation, headline brainstorms, copy-editing, format translation (article → newsletter → social).
- **Edge:** synthesizing across multiple sources with conflicting framings.
- **Outside:** original reporting (interviews, document access), voice with sustained idiosyncrasy, fact-claims that require source-of-record verification.

### Design (UX, visual)
- **Inside:** moodboard generation, variation on a brief, design-token / style-guide drafting, icon and illustration first passes.
- **Edge:** layout decisions on real product data, accessibility-trade-off design.
- **Outside:** anything requiring familiarity with the actual user base or the surrounding product context the AI has not seen.

### Marketing / sales
- **Inside:** ad copy variants, segmentation hypotheses, persona drafts, follow-up email templates.
- **Outside:** account-specific positioning that requires institutional memory, judgment about timing and trust-building in real relationships.

### Research (academic, market, scientific literature)
- **Inside:** summarization of long papers (Mollick's own admitted use), generating reading lists, translating jargon across subfields.
- **Outside:** evaluating novelty against the actual frontier of a field (where the AI's training cutoff matters), reasoning over evidence quality, conducting experiments.

The pattern across all professions: **AI handles "first draft of known-shape work" well and handles "judgment under uncertainty with downside risk" badly.** This is the practical heuristic; mapping is how you locate the actual edge for your specific tasks.

## How to Invest Mapping Effort

Time spent mapping is a real cost. The investment logic:

### Prioritize high-volume, low-stakes-of-error tasks first
These are where AI's expected value is highest and the downside is bounded. Mollick's "Delegated Task" category — tedious, repetitive, low-importance — is where mapping pays off fastest. Discover the inside-frontier tasks here, redeploy the freed time.

### Avoid early reliance on tasks where you'd be the only check
For tasks where there's no downstream reviewer (you are the senior partner, the tenured professor, the staff engineer of record), the "falling asleep at the wheel" risk is highest. Map carefully; preserve manual practice; treat AI as a second opinion, not the first answer.

### Identify your "Just Me" tasks explicitly
Mollick's category — tasks you choose to keep human even if AI could do them — is not a mapping output but a mapping input. Voice, relationship-building, ethical decisions, anything where the *process* of doing it matters as much as the output. Decide before you delegate, not after.

### Re-map after each model release
Frontier movement is the single biggest reason cached judgments fail. A task that was outside the frontier on GPT-4 may be inside on GPT-5. Schedule mapping reviews — quarterly is roughly right for current model release cadence — and treat them as professional development, not optional experimentation.

### Map across the Centaur and Cyborg modes
Mollick's distinction: **Centaur** work has a clear hand-off (you do A, AI does B); **Cyborg** work intertwines (AI completes your sentence, you redirect, repeat). The frontier looks different in each mode. The same task that fails when fully delegated may succeed when iteratively co-produced. Mapping should include both modes, not just one.

## What Investment Mapping Does *Not* Replace

The mapping investment locates the frontier; it does not by itself solve the [[cognitive-atrophy-and-ai|cognitive atrophy]] problem. Mapping tells you that AI is good at a task; the question of whether you should *let* AI do that task — especially during your formative years in the discipline — is separate. Mollick's "be the human in the loop" is necessary but underdetermined; the atrophy page argues that the threshold between augmentation and atrophy shifts with expertise level.

Combined recommendation:

- **Novices** should map cautiously and deliberately preserve unaided practice on tasks where the expert intuition is still forming.
- **Senior practitioners** can map aggressively and delegate broadly — the underlying judgment is already built and can catch AI errors.
- **Everyone** should treat the personal frontier map as a living document, owned by them, not by their employer or industry analyst.

The mapping investment is high-leverage because the cost is small (an afternoon's experimentation) and the asset is durable (a personal protocol that compounds over a career as the frontier moves). It is also non-substitutable: no vendor, employer, or research report can give you your specific map.

## Source
- `raw/books/Ethan Mollick - Co-Intelligence_ Living and Working With AI (2024, Penguin Publishing Group).epub` — especially Ch. 3 ("Four Rules for Co-Intelligence") and Ch. 6 ("AI as a Coworker")

## Related Topics
- [[jagged-frontier]] — the concept this page operationalizes
- [[living-and-working-with-ai]] — the broader Mollick framework
- [[ethan-mollick]] — the researcher
- [[cognitive-atrophy-and-ai]] — the cost side of aggressive mapping
- [[large-language-models]] — the technology defining the frontier
