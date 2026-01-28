

# LLM-Driven Feature Engineering for Risk Assessment from Unstructured Text

## Overview

This project investigates how Large Language Models (LLMs) can be systematically
used to transform unstructured narrative text into **structured, interpretable,
and analysis-ready features** aligned with predefined risk assessment
frameworks.

Rather than focusing on prediction or model accuracy, the project emphasizes
**feature engineering as the central analytical task**, treating LLMs as
controlled information extractors capable of producing consistent, schema-based
outputs.

The work was completed as part of a graduate-level university course and is
intended for academic and educational purposes.

---

## Problem Context

Many analytical domains rely on free-form textual data such as narratives,
descriptions, or reports. While such data contains rich contextual information,
it presents significant challenges:

- Lack of consistent structure
- High manual effort required for annotation
- Difficulty in applying statistical or quantitative analysis
- Loss of interpretability when using black-box models

At the same time, established assessment frameworks exist that define **what
should be measured**, but not **how to reliably extract those measurements from
text**.

This project addresses this gap by exploring whether LLMs can be used to
*operationalize* conceptual frameworks by converting unstructured text into
explicit, well-defined features.

---

## What This Project Does

At a high level, the project performs the following:

1. **Defines a structured taxonomy** of analytically meaningful features grounded
   in recognized assessment dimensions
2. **Designs constrained, instruction-based prompts** that guide an LLM to
   extract those features from raw text
3. **Standardizes LLM outputs** into a clean, tabular feature schema
4. **Demonstrates how these features enable downstream analysis**, aggregation,
   and reporting without reliance on raw text

The emphasis is on **clarity, reproducibility, and interpretability**, rather
than automation or scale.

---

## Key Design Principles

Several principles guided the project design:

### 1. Feature-First Thinking
Instead of asking *“What can the model predict?”*, the project asks:
> *“What measurable signals are conceptually meaningful, and how can they be
reliably extracted?”*

Every feature is:
- Explicitly defined
- Justified within the taxonomy
- Intended to be interpretable by non-technical stakeholders

### 2. Taxonomy-Driven Extraction
All extraction is grounded in a predefined taxonomy that:
- Groups related concepts into logical categories
- Separates behavioral, cognitive, contextual, and historical dimensions
- Prevents uncontrolled or ambiguous outputs from the LLM

### 3. Prompt as Analytical Instrument
The LLM prompt is treated as an **instrument**, not a query:
- Instructions are explicit and constrained
- Output format is standardized
- Ambiguity is minimized through clear definitions and examples

### 4. Separation of Concerns
The project deliberately separates:
- Conceptual design (taxonomy)
- Extraction logic (prompt)
- Representation (feature schema)
- Interpretation (analysis and reporting)

This separation improves transparency and auditability.

---

## Methodology in Detail

### Taxonomy Development
A structured taxonomy was developed to represent the key dimensions relevant to
risk assessment in narrative text. Each category was broken down into discrete,
observable indicators that could be expressed as features.

This step ensured that:
- Abstract concepts were translated into measurable variables
- Feature scope was clearly bounded
- Downstream analysis remained interpretable

### Prompt-Driven Feature Extraction
A carefully designed prompt instructs the LLM to:
- Analyze a given narrative
- Identify signals corresponding to each taxonomy category
- Output feature values in a structured, consistent format

The prompt prioritizes:
- Deterministic instructions
- Explicit constraints
- Consistent labeling and naming

### Feature Schema Construction
LLM outputs were converted into a finalized feature schema that:
- Defines feature names and categories
- Provides clear definitions for each variable
- Supports encoding, aggregation, and comparison

This schema functions as the **contract** between unstructured text and
quantitative analysis.

---

## Outputs and Artifacts

The repository contains the following deliverables:

- **Executive Summary** outlining objectives, approach, and conclusions
- **Taxonomy Documentation** detailing conceptual structure and feature logic
- **LLM Prompt Specification** describing extraction instructions and constraints
- **Appendices** with supporting tables and extended explanations
- **Presentation Decks** for academic evaluation
- **Final Feature Schema** capturing all engineered variables

No raw text or sensitive datasets are included.

---

## Results and Insights

The project demonstrates that:

- LLMs can be used as **structured feature extractors** when guided by strong
  taxonomies and explicit prompts
- Feature consistency improves significantly when output constraints are applied
- Interpretability is preserved when features are explicitly defined and grouped
- Documentation and schema design play a critical role in LLM-based workflows

Rather than replacing analytical reasoning, LLMs act as a **scaling mechanism for
feature engineering**, enabling structured analysis of narrative data.

---

## Key Takeaways

- Feature engineering remains essential, even in LLM-driven systems
- Taxonomy design directly impacts analytical quality
- Prompts should be treated as analytical instruments, not ad-hoc queries
- Structured outputs enable transparency, auditing, and reuse
- LLMs are most effective when constrained, not when left open-ended

---

## Limitations and Academic Scope

- This is an academic, exploratory project
- No claims are made regarding real-world deployment or clinical use
- Results depend on prompt design and conceptual framing
- Findings should be interpreted within an educational context

---

## Academic Use and Disclaimer

This project was completed as part of a university course and is intended solely
for academic and educational purposes. It does not provide diagnostic,
predictive, or operational recommendations.

