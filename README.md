# AI-paper-writing-skill

A platform-independent English skill for drafting, revising, and reviewing scientific research papers, especially AI/ML and computational method papers.

The skill organizes a manuscript around a coherent research narrative:

**Observation -> research question -> objective -> method -> experiment -> evidence -> conclusion.**

## Eight writing standards

1. **Method:** derive the design from the research problem and explain mathematical formulations and mechanisms. Link a GitHub repository for code and reproduction instructions.
2. **Prose:** write directly, objectively, and specifically, without defensive framing or empty promotional language.
3. **Core narrative:** connect the observed phenomenon, research question, design decisions, experiments, and findings throughout the paper.
4. **Introduction:** establish background, observations, motivation, research gap, objectives, core idea, and contributions.
5. **Related Work:** objectively organize prior problems, methods, extensions, and technical directions.
6. **Experiments:** give each test an explicit question, setup, traceable results, interpretation, and answer.
7. **Experimental synthesis:** integrate the findings into an overall answer to the research question.
8. **Conclusion:** connect the problem, method, key numerical evidence, research findings, and concrete future directions.

## Use with an AI assistant

Provide [SKILL.md](SKILL.md) as instructions to an assistant that can read Markdown files. Include the `references` folder when the assistant supports file access, or attach the relevant reference alongside the skill.

Example request:

> Follow SKILL.md to revise this scientific manuscript. Preserve the research facts, apply the eight writing standards, and keep editorial comments separate from manuscript prose.

For a review:

> Review this manuscript using SKILL.md. Identify the relevant passage, the concrete writing or reasoning issue, and an actionable revision. Verify claims and numbers against the supplied research materials.

Supply the manuscript or notes, actual method details, experimental records, literature sources, and target publication format relevant to your task. The instructions are in English; manuscript output can use the language you request.

## Files

```text
AI-paper-writing-skill/
|-- README.md
|-- SKILL.md
`-- references/
    |-- examples.md
    `-- source-notes.md
```

- [SKILL.md](SKILL.md): workflow, eight standards, and final manuscript checks.
- [Examples](references/examples.md): preferred prose and revision patterns.
- [Source notes](references/source-notes.md): GitHub resources informing the checks.

## Research integrity

Use actual research records and verified sources. Keep numerical results, experimental settings, citations, figures, and conclusions consistent with those materials. Obtain missing scientific information from the researcher.

## Compatibility

The package uses Markdown instructions and simple skill metadata. It contains no provider-specific configuration or required API integration. Use the instruction-loading mechanism supported by your assistant or editor.
