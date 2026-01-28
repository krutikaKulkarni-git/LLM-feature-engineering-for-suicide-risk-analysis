# LLM-Driven Feature Engineering for Suicide Risk Analysis from Reddit Text

## Project Overview

This academic project explores how Large Language Models (LLMs) can be used as
**controlled, interpretable feature extractors** to transform unstructured,
user-generated text into structured variables suitable for quantitative
analysis.

Using narrative data from Reddit’s **/r/SuicideWatch** subreddit, the project
designs a **taxonomy-driven, prompt-based feature engineering pipeline** that
extracts clinically and behaviorally meaningful signals related to suicidal
ideation, planning behaviors, attempts, mental health traits, reasons/motives,
and coping mechanisms.

Rather than focusing on prediction or automated decision-making, the project
centers on **feature engineering, interpretability, and analytical rigor**.
The work was completed as part of a graduate-level university course.

> **Data Note**  
> Due to the sensitive nature of the content, the dataset used in this project
> cannot be shared publicly. This repository contains documentation, feature
> schemas, prompt specifications, and analysis summaries so the methodology is
> reproducible without exposing raw user data.

---

## Problem Context and Motivation

Many real-world domains rely on free-form textual data such as narratives,
descriptions, and self-reported experiences. While these texts contain rich and
valuable information, they pose significant analytical challenges:

- Lack of consistent structure
- High manual effort required for annotation
- Difficulty applying statistical or quantitative methods
- Reduced interpretability when using black-box models

In mental health and risk assessment contexts, established conceptual and
clinical frameworks define **what should be assessed**, but translating
unstructured narratives into structured indicators remains labor-intensive and
inconsistent.

This project addresses that gap by investigating whether **LLMs can operationalize
predefined assessment frameworks**, converting narrative text into explicit,
well-defined, and interpretable features suitable for downstream analysis.

---

## What This Project Does (End-to-End)

At a high level, the project implements the following workflow:

### 1. Thread-Based Narrative Construction
- Reddit threads are organized by grouping the original post with comments from
  the same author.
- The unit of analysis becomes a **user-level narrative within a thread**,
  providing richer context for feature extraction.

### 2. Taxonomy-Driven Feature Definition
- A structured taxonomy is designed to represent analytically meaningful
  dimensions of suicide risk and mental health.
- Features are grouped across dimensions such as:
  - Suicidal or self-harm ideation
  - Preparatory planning behaviors
  - Suicide attempts
  - Methods mentioned
  - Reasons and motivating factors
  - DSM-5–aligned mental illness traits
  - Coping mechanisms and treatment indicators
- Each feature is explicitly defined to preserve interpretability.

### 3. LLM-Driven Feature Extraction (Prompt as Instrument)
- A carefully designed, constraint-based prompt instructs the LLM to:
  - Analyze narrative text
  - Identify signals aligned with the predefined taxonomy
  - Output results in a structured, schema-consistent format
- The prompt is treated as an **analytical instrument**, not an ad-hoc query,
  emphasizing determinism, clarity, and reproducibility.

### 4. Data Cleaning and Standardization
- Rows with critical missing fields are removed; invalid authors are excluded.
- Timestamps are standardized; non-critical missing values are filled with
  explicit “None” indicators.
- Categorical features are one-hot encoded to enable statistical analysis.

### 5. Downstream Analysis
- Exploratory analysis is conducted across behavioral signals and demographics
  (where available).
- Statistical tests evaluate relationships between planning behaviors and
  suicide attempts.
- Results emphasize **interpretation and insight**, not prediction.

---

## Repository Structure

.
├── README.md
├── docs/
│ ├── Executive_Summary.docx
│ ├── Taxonomy.docx
│ ├── Prompt_for_LLM.docx
│ └── Appendices.docx
├── slides/
│ ├── Class_Presentation.pptx
│ └── Detailed_Presentation_Deck.pptx
└── schema/
└── Final_Feature_list.xlsx


### Folder Descriptions
- **docs/**: Conceptual design, taxonomy, prompt specification, and supporting
  analysis
- **slides/**: Presentation materials used for academic evaluation
- **schema/**: Final engineered feature list used for analysis and reporting

---

## Key Results and Findings (Highlights)

### Dataset Scale and Cleaning
- Initial dataset contained approximately **140k unique users** and **363k rows**.
- After cleaning and validation:
  - Users reduced to **~84,798**
  - Rows reduced to **~225,185**
- Cleaning ensured analytical reliability and consistency.

### Prevalence of Suicidal / NSSI Signals
- Among cleaned users, **~92.6% (78,515 / 84,798)** mentioned suicidal or
  self-harm thoughts at least once.

### Planning and Suicide Attempts
- Users reporting preparatory planning exhibited higher attempt rates:
  - No-plan group: **~12.3%**
  - Plan group: **~19.9%**
- Statistical testing indicates a significant association between planning and
  attempts, with odds of attempting approximately **1.78× higher** for users
  who reported planning behaviors.

### Reasons and Mental Health Traits
- Approximately **80%** of users cited at least one reason or motive for suicidal
  thoughts.
- Family/friend issues and emotional pain emerged as dominant drivers, with
  observable gender differences.
- DSM-5–aligned categorization shows mood and anxiety disorders as the most
  frequently cited mental health traits; mood disorders dominate among users
  who reported attempts.

### Coping and Treatment Signals
- Only a small subset of users reported healthy coping mechanisms.
- Creative and hobby-based coping appeared most frequently among those who did.
- Treatment signals (e.g., medication, therapy) were limited in frequency, so
  conclusions are descriptive rather than causal.

---

## Key Design Principles

- **Feature-first thinking**: focus on what should be measured, not what to
  predict
- **Taxonomy-driven extraction**: constrain LLM outputs to predefined concepts
- **Prompt as analytical instrument**: explicit instructions and structured
  outputs
- **Separation of concerns**: taxonomy, extraction, schema, and interpretation
  are deliberately decoupled

---

## Key Takeaways

- LLMs can function effectively as **structured feature extractors** when
  constrained by strong taxonomies and prompts
- Feature engineering remains a critical analytical skill in LLM-based workflows
- Interpretability and reproducibility improve with explicit schema design
- Narrative text can be analyzed quantitatively without exposing raw content
- LLMs are most useful when **guided and constrained**, not used as black boxes

---

## Dataset and Privacy

This project uses sensitive, user-generated mental health content.
To ensure ethical and responsible use:

- Raw text, usernames, and full datasets are **not included**
- Only documentation, schema, prompts, and aggregated results are shared
- Dataset access may be discussed privately for academic review if required

---

## Academic Scope and Disclaimer

- This is an exploratory academic project
- It is not intended for clinical, diagnostic, or operational use
- No automated intervention or risk scoring is proposed
- Findings should be interpreted strictly within an educational context
