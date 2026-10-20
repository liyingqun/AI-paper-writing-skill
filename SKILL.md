---
name: scientific-paper-writing
description: Draft, revise, or review scientific research manuscripts using an observation-driven research narrative, mathematical method descriptions, objective related work, question-driven experiments, and direct evidence-based prose. Apply especially to AI/ML and computational method papers, including checks for AI-generated writing errors.
---

# Scientific Paper Writing

Use the eight standards below to produce a coherent scientific manuscript. Follow the target publication template when arranging sections, while preserving the research logic. These instructions are platform-independent and can be used by any AI assistant that can read Markdown instructions.

Write manuscript prose in the requested language; this skill's instructions are in English.

## Working procedure

1. Identify the requested task: draft, revise, review, or outline. Read the supplied manuscript, research notes, references, methods, experiment records, and target format relevant to that task.
2. Establish one central research question and a compact evidence map: observed phenomenon -> question -> objective -> method component -> experiment -> result -> conclusion. Use the map internally unless the user requests it.
3. Apply the eight standards below to the requested scope. For a paragraph edit, check its local role and terminology; for a full manuscript, check the complete narrative and cross-section consistency.
4. Verify factual content against source material. Obtain missing information that changes scientific content, or identify it briefly outside the manuscript. Continue work on supported material. Do not fill factual gaps with invented content.
5. Deliver the requested manuscript or review. Keep editorial commentary separate from manuscript prose. For reviews, identify the passage, concrete problem, and actionable revision.

Read [references/examples.md](references/examples.md) when drafting or correcting passages that need examples of the preferred style. Consult [references/source-notes.md](references/source-notes.md) when the user requests the provenance of these checks.

## 1. Method: derive the design from the research problem

Organize each substantive method component as:

**Target problem -> design rationale -> mathematical formulation -> variable and mechanism explanation -> role in the complete method.**

- Define the problem, inputs, outputs, assumptions, symbols, and dimensions needed to understand the method.
- Explain why a component is introduced before presenting its equation. Explain how the equation implements the intended mechanism afterward.
- Describe the method through research principles, mathematical relationships, and interacting components. Use equations to specify real relationships, not to decorate prose.
- Keep terminology, notation, dimensions, and component names consistent throughout the manuscript, diagrams, and tables.
- Ensure the description matches the actual method and implementation supplied by the researcher.
- Put source code, execution commands, function-call instructions, and operational tutorials in a **GitHub repository linked from the paper**. The repository README should cover environment setup, data preparation, training, evaluation, and reproduction of the reported results.
- Retain the scientific definitions and experimental settings needed to understand and assess the research in the paper. A repository link complements this content.
- Use an actual supplied or verified GitHub URL. If the URL is missing, request it or note the missing link outside the manuscript. Creating a public repository or uploading code requires the user's authorization for that action.

Check for AI-generated code walkthroughs disguised as methodology, unexplained equations, invented components, and formulas disconnected from design decisions.

## 2. Prose: direct, objective, specific, and free of defensive framing

State research premises, purposes, designs, observations, measurements, and findings directly.

- Remove anticipatory rebuttals, apologetic concessions, self-justification, self-praise, and responses to imaginary reviewers.
- State assumptions and experimental conditions affirmatively where they define the research setting.
- Avoid unsupported speculation and gratuitous hedging. Use the exact statement established by the source material.
- Preserve actual measurements and statistical reporting, including reported variability. Describe them as results without adding defensive commentary.
- Replace generic praise and vague adjectives with named mechanisms, metrics, comparison conditions, and measured differences.
- Reserve statistical significance terminology for an actual reported statistical analysis.
- Remove filler such as "it is worth noting," "important insights," and "paving the way" when it contributes no research information.

This is a prose standard: maintain fidelity to the supplied research facts while writing them directly.

## 3. Core: maintain an observation-driven research narrative

Build motivation from **what was observed and what question that observation raises**.

Maintain the chain:

**Observation -> research question -> objective -> design rationale -> method -> experimental test -> evidence -> research answer.**

- State the central question precisely enough to guide both method design and evaluation.
- Keep the abstract, introduction, method, experiments, and conclusion aligned with that question.
- Give each paragraph one clear function. Connect paragraphs through substantive reasoning.
- Connect every component to its purpose, every experiment to a question or claim, and every conclusion to the corresponding evidence.
- Preserve stable research objectives and contribution wording across sections.

Check for independently fluent sections that tell different research stories, unexplained logical jumps, and transitions that substitute for reasoning.

## 4. Introduction: establish the problem and contribution

Use this progression:

**Background -> concrete observation -> motivation and research question -> literature-grounded gap -> objective -> core idea -> contributions.**

- Background establishes the research setting and its importance.
- Observation states the specific phenomenon that generated the question.
- Motivation explains why investigating that phenomenon matters.
- Gap identifies the precise research position to be addressed, grounded in verified literature.
- Objective states what the study will answer or accomplish.
- Core idea explains how the proposed approach addresses the problem at a conceptual level.
- Contributions state new methods, theoretical results, findings, or resources and map to material actually present later in the paper.

Describe research outputs rather than listing activities such as "we conducted extensive experiments." Keep implementation recipes and detailed hyperparameters in their appropriate sections.

Check for generic technology-trend openings, long background without a concrete observation, vague novelty, and contributions that duplicate one another.

## 5. Related Work: objectively organize research development

Group literature by research problem or technical direction. Within each group, explain:

**Problem addressed -> researchers and representative methods -> subsequent extensions or enhancements -> resulting technical directions.**

- Explain relationships among studies instead of producing isolated paper summaries.
- Present research objectives, mechanisms, and developments through factual descriptions and citations.
- Keep this section focused on prior research. Develop the present method in the Introduction and Method.
- Avoid an evaluative list of shortcomings or promotional comparisons with the present method.
- Use prose for the literature synthesis; place detailed mathematical development in Method.
- Verify author names, years, titles, method descriptions, and bibliographic entries. Confirm that each cited work supports the associated statement.

Check for fabricated citations, citation-content mismatches, conflated methods, repetitive promotion, and chronological lists with no conceptual organization.

## 6. Experiments: answer explicit questions with traceable evidence

Organize each experiment as:

**Question -> reason for the test -> experimental setup -> table or figure -> key observation -> interpretation -> answer.**

- Explain what the test is intended to establish and why its comparison and metric answer that question.
- Specify relevant datasets, splits, baselines, metrics, training settings, tuning and measurement procedures, repetitions, and computational resources from actual records.
- Maintain comparable conditions and identify the controlled variables.
- Use main comparisons for overall performance, ablations for component analysis, and additional tests for explicitly stated questions.
- Source all numerical results from actual experiment records. Check calculations, units, percentage-point versus relative changes, and metric direction.
- Use tables and figures suited to the question. Verify that every referenced artifact exists and contains the stated data.
- Interpret the important differences and trends, then connect them to the research question. Avoid narrating every table cell.
- Keep numerical values consistent across logs, tables, captions, abstract, and prose.

Check for experiments selected without a research purpose, invented settings or results, mismatched comparisons, unsupported explanations, and nonexistent or mislabeled figures.

## 7. Experimental synthesis: combine the findings

End the experimental chapter with a synthesis, or use the corresponding Discussion section required by the target format.

Use this progression:

**Main findings -> component findings -> additional findings -> relationship among the findings -> overall experimental conclusion.**

- Reconnect the evidence to the research claims introduced earlier.
- Explain what each experiment contributes to the combined research answer.
- Identify the pattern established across tests and its research meaning.
- Use findings already presented in the chapter.
- Write an integrated conclusion rather than a sequence of table summaries or a generic statement of success.

## 8. Conclusion: deliver the research answer

Use this progression:

**Research context and question -> core method -> key numerical evidence -> research conclusion -> concrete future development.**

- Briefly recall the problem and objective.
- Summarize the defining design, then select the results that best express the main findings.
- State the knowledge gained and the answer to the original question.
- Derive future directions from the research findings: a specific new task, condition, mechanism, or application.
- Keep terminology, numbers, and claims aligned with the manuscript.

Check for copied abstracts, method-only recaps, new results introduced at the end, and generic future work such as "improve performance" without a concrete direction.

## Final manuscript check

Before delivery, inspect the requested scope for:

- A consistent observation-question-method-evidence-conclusion chain.
- Verified research facts and citation-content matches.
- Clear component purposes, equations, definitions, and stable terminology.
- Explicit experimental questions, traceable numbers, and consistent comparisons.
- Correct figure/table references, captions, units, and document structure.
- Direct prose with no defensive framing, filler, or repeated self-praise.
- An actual GitHub repository link when code availability is stated.
- A synthesis and conclusion that answer the research question using the presented findings.
