# schol-rs-exemplars

I've got AI to transcribe handwritten PDFs to readable texts.

You could paste the link to this repository (https://github.com/Cirrow/schol-rs-exemplars) to any LLM of your choice, and have them analyse the texts for you, find patterns, etc. Or you could get them to generate a structured plan for your essay based on the exemplar answers.

Visit the [diagnostics](https://github.com/Cirrow/schol-rs-exemplars/tree/main/diagnostics) folder to view what the LLMs generated based on the files of this repository. It contains analyses of these exemplars - common patterns, strategies, and things to avoid, etc.


## File structure
You can browse each answers grouped by year. They each contain each exemplar answers, raw and formatted. They have no difference. One just looks better than the other.
Tildes (`~`) represent a strikethrough that were present in the original handwriting.


## Example prompt

<blockquote>
# ROLE AND STANCE
You are a strict senior examiner and academic analyst reviewing exemplar essays for NZ Scholarship Religious Studies. Be critical, but only criticise what the texts and the official standard support. Do not manufacture flaws to sound rigorous, and do not flatter. If the evidence for a point is thin, say so and move on.

# TASK
Analyse the exemplar essays in the project context (linked GitHub repository) as one corpus of high-performing writing. Produce a diagnostic report that identifies recurring and non-recurring features, explains their likely function, and converts them into usable guidance for a student writing under timed exam conditions.

# STANDARDS AND SOURCES
- The NZ Scholarship Religious Studies performance standard (text file in project context, published by the Ministry of Education) is the primary benchmark. Where the standard is silent or ambiguous, state that explicitly and reason from the closest applicable principle rather than inventing a criterion.
- Marking criteria to apply: sustained argument, accurate and relevant evidence, critical engagement, coherent structure, direct response to the question. Do not infer quality from style alone.
- If any file cannot be read or is truncated, state this at the start and exclude it. Never infer an essay's content from its title or from other essays.

# BEFORE ANALYSIS: CORPUS INVENTORY
Produce a table: essay ID, topic/question, approximate length, genre or format notes, and any official grade or marker comment if present. If no marks are given, state that quality is assumed from "exemplar" status only (the title of the files, if named "scholarship", "outsanding" or "topscholar", those are the grades). Flag essays that are not directly comparable (if any) and say how that limits comparison. State the corpus size and note that small samples limit any generalisation.

Essay IDs should be in this format: YY-GG where YY is a two-digit year ending ("25" for 2025, etc.) and GG is the grade (S for Scholarship, O for outsdanding, T for topscholar).

Note: 25-Je, 25-Jo and 25-Sa are at scholarship level mark (14-15).

# METHOD
1. Compare across essays rather than summarising each one.
2. For every substantive claim, cite the essay ID, quote a short exact phrase or sentence, and give its location by essay ID and, where possible, paragraph number or a distinctive preceding phrase. Quote verbatim. Never paraphrase inside quotation marks or invent a quotation. If you cannot locate an exact quote, omit the claim.
3. Label every pattern:
   - **Corpus-wide** (most or all essays)
   - **Recurrent** (several essays)
   - **Individual technique** (one or two essays)
   - **Absence** (a plausible high-scoring feature none of the essays use)
4. Do not assume any shared structure, tripartite framework, roadmap, or paragraph model. Test each against the texts. Where a pattern is inconsistent, say so and propose what explains the variation (topic, year, tradition, question type).
5. Vocabulary, famous quotations, and citation density are not inherently good. Judge each by whether it advances the argument.
6. If evidence for a section is thin, write "insufficient evidence in corpus" instead of filling the slot. A shorter, honest section is better than a padded one.
7. Separate **transferable** findings (apply to any question) from **topic-specific** ones (depend on the religious tradition or question).

# ANALYSE

## 1. Argument architecture
- How is the central claim established in the introduction? Classify as direct, qualified, question-led, or other.
- What organisational logic appears: thematic, chronological, theoretical, dialectical, problem-solution, or mixed?
- How do writers signal movement between sections and manage competing perspectives?
- Quote and explain the 2-3 most effective transitions, and say why they work logically, not just stylistically.

## 2. Paragraph mechanics
Reconstruct the move sequence of 3-5 representative paragraphs (claim, evidence/interpretation, qualification or counter-view, implication/link). State whether this sequence is common or confined to a few essays. Assess:
- Ratio of evidence to commentary, and what the commentary actually does
- Precision of references, quotations, examples and terminology
- **Originality of examples:** are the case studies or sources distinctive or standard? Does the writer extract a meaningful argument from them, or only illustrate? Does original material correlate with stronger argument in this corpus, or are standard examples used just as effectively?
- **Language:** is vocabulary precise, ornamental, or vague? Compare plain-style and elaborate-style passages. Does elaborate phrasing add precision, or could plain prose do the same work?

## 3. What distinguishes stronger execution
Identify practices that appear to raise quality, such as turning evidence into argument, anticipating objections without abandoning the main claim, using theory or case material to answer the exact question, and controlling scope toward a defensible final judgement. Give at least one concrete textual example for each. Where a practice appears in only one essay, label it as such and do not present it as a rule.

## 4. Weaknesses and missed potential
Identify limitations such as:
- Frameworks imposed where they fit only partially
- Assertions unsupported by textual evidence
- Transitions that gesture at connection without establishing it
- Conclusions that restate instead of resolving the central tension
- Breadth bought at the cost of depth
- Over-reliance on quotation-dropping, name-dropping, or ornate phrasing

Rate each as common / occasional / rare, give examples, and say why an examiner working from the performance standard would or would not penalise it.

## 5. Conditional writing blueprint
Provide a practical template that is conditional, not universal, and realistic for a timed essay:
1. **Introduction:** functional moves, with alternatives where the corpus shows more than one approach
2. **Body block:** a repeatable 4-6 move sequence
3. **Counter-view handling:** how to engage opposition without derailing the thesis
4. **Synthesis:** how to tie evidence back to the question
5. **Conclusion:** how to reach a definite, evidenced judgement without quote-dumping or generic philosophy

For each element, note whether it is corpus-wide or drawn from a minority of essays.

# OUTPUT RULES
- Use Markdown headings, concise bullets, and tables where useful.
- Prioritise specific textual evidence over general writing advice. If a point cannot be supported by a quotation or an identifiable structural move, omit it.
- Do not pad. Every paragraph must contribute a distinct finding.
- Length: about 3,000 words with a bit of wiggle room on the ceiling, with the inventory table and checklists not counted. Be comparative and selective; do not summarise essays sequentially.
- End with two checklists:
  1. **Knowledge checklist:** content, concepts and sources a student should have secured before the exam.
  2. **In-exam reminders:** a short list of moves to check while writing under time pressure.
- Finish with a brief **Limitations** note: what this corpus cannot tell us (for example, marker comments, mark allocations, or how typical these essays are).
</blockquote>
