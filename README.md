

# LLM-Driven Feature Engineering for Risk Assessment from Unstructured Text

This repository contains the documentation, presentation materials, and feature
schema for a graduate-level class project focused on converting unstructured
text into structured, analytically meaningful features using Large Language
Models (LLMs).

The project emphasizes **feature engineering, taxonomy design, and prompt-driven
extraction**, rather than model training or deployment.

---

## 1. Project Motivation

Many real-world domains rely on unstructured textual data (e.g., narratives,
reports, free-text responses) that are difficult to analyze using traditional
statistical or machine learning techniques.

In sensitive and high-stakes contexts, structured assessment frameworks exist,
but mapping free-form text to these frameworks is labor-intensive and
inconsistent.

This project explores how **LLMs can be used as structured feature extractors**
to bridge this gap by:
- Translating unstructured text into predefined analytical features
- Preserving interpretability and alignment with domain frameworks
- Enabling downstream quantitative analysis without exposing raw text

---

## 2. Project Objective

The primary objectives of this project are:

- To design a **taxonomy of risk-related features** grounded in established
  assessment dimensions
- To develop **prompt-driven LLM instructions** that reliably extract these
  features from unstructured text
- To produce a **clean, structured feature schema** suitable for analysis and
  reporting
- To evaluate the feasibility and consistency of LLM-based feature engineering
  for academic analytical workflows

---

## 3. Methodology Overview

The project follows a **documentation-first, analysis-ready** approach.

### 3.1 Conceptual Design
- Defined a structured taxonomy representing key behavioral, cognitive, and
  contextual dimensions
- Mapped abstract concepts into measurable, discrete features
- Ensured interpretability and logical grouping for downstream analysis

### 3.2 Prompt-Driven Feature Extraction
- Designed structured prompts instructing the LLM to:
  - Read unstructured narratives
  - Identify relevant signals aligned with the taxonomy
  - Output features in a consistent, structured format
- Focused on reproducibility, clarity, and constraint-based prompting

### 3.3 Feature Engineering Output
- Converted LLM outputs into tabular, schema-driven feature representations
- Standardized feature naming, categories, and definitions
- Prepared features for aggregation, encoding, and statistical analysis

---

## 4. Repository Structure


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

#### `docs/`
Contains the core written documentation:
- **Executive Summary** – high-level overview, objectives, and conclusions
- **Taxonomy** – conceptual framework and feature categorization
- **Prompt for LLM** – detailed prompt design and extraction logic
- **Appendices** – supplementary analysis, tables, and clarifications

#### `slides/`
Presentation materials used for academic evaluation:
- A concise in-class presentation
- A detailed deck covering methodology, examples, and findings

#### `schema/`
The finalized feature schema:
- Master list of engineered features
- Feature categories, definitions, and intended interpretation

---

## 5. Data Availability

Due to the sensitive nature of the subject matter, **raw textual data and
derived datasets are not included in this repository**.

This repository focuses on:
- Methodology
- Feature design
- Documentation and analytical structure

Data may be made available upon academic request where appropriate.

---

## 6. Results and Outcomes

Key outcomes of the project include:

- A clearly defined **feature taxonomy** that translates abstract risk concepts
  into structured variables
- A **prompt framework** capable of producing consistent, schema-aligned feature
  outputs from unstructured text
- A finalized **feature list** suitable for:
  - Statistical analysis
  - Aggregation and encoding
  - Dashboarding and reporting
- Demonstration of LLMs as **feature engineering tools**, not black-box predictors

The results indicate that prompt-driven LLMs can support structured analytical
workflows when combined with strong taxonomy design and clear constraints.

---

## 7. Academic Context and Limitations

- This project was completed as part of a university course.
- It is intended for **educational and exploratory purposes only**.
- No clinical, diagnostic, or operational claims are made.
- Findings should not be interpreted as production-ready or decision-making
  systems.

---

## 8. Key Takeaways

- LLMs can function as **structured information extractors**, not just generators
- Strong taxonomy design is critical for interpretability
- Feature engineering remains a central analytical skill even in LLM-driven
  workflows
- Documentation and schema design are as important as modeling

---

## 9. License

This repository is shared for academic and educational review only.
