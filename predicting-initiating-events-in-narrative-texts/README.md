# Predicting Initiating Events in Narrative Texts Using Machine Learning

This project explores how computer models can help identify Initiating Events in stories — the part of a narrative where something happens that sets the story in motion.  
By analyzing features of students' writing, the model learns patterns that make an event more or less likely to be recognized as an Initiating Event.

---

## Overview

- **Goal:** Use language and writing features to automatically predict whether a story's section contains an Initiating Event (IE).  
- **Data:** Narrative writing samples that include linguistic and descriptive measurements for each section.  
- **Approach:** Several machine learning models were tested; the Random Forest model gave the best overall results.

---

## What the Model Does

The Random Forest model looks at dozens of features that describe how a story is written — such as vocabulary variety, sentence structure, and how well the story flows.  
It then predicts whether a given part of the text is an Initiating Event.

- **Best model:** Random Forest  
- **Cross-validated accuracy:** ~58.6%  
  (The model correctly identifies the Initiating Event a little more than half the time — meaningful for early-stage educational analysis.)

---

## Important Writing Features

The model found several characteristics that most strongly influence whether a section is recognized as an Initiating Event:

| Feature | What It Represents |
|---------|-------------------|
| DESWC | Amount of descriptive language used in the text |
| PCNARp | How smoothly the story progresses from one idea to another |
| LSAGN | Sophistication and variety of word choice |
| SYNLE | Sentence structure and grammatical complexity |
| DESWLsyd | Diversity of descriptive words |
| PCDCz | Overall story cohesion and connection between sentences |
| DRPP | Use of pronouns and linking words that maintain flow |
| DESSC | Consistency and meaning of descriptive language |
| SMCAUSlsa | Logical or causal links between ideas in the story |
| LDTTRc | Vocabulary diversity and richness |

These elements together help the model decide whether a text segment functions as a true "event starter" in the story.

---

## Main Findings

- Stories with clear, detailed descriptions and logical flow are more likely to contain strong Initiating Events.  
- Writing that shows higher vocabulary variety and sentence complexity tends to be easier for the model to recognize as containing an Initiating Event.  
- The model provides useful insights for teachers or researchers studying language development and storytelling skills.

---

## Repository Contents

| File | Description |
|------|-------------|
| `Predicting Initiating Events in Narrative Texts.ipynb` | Main notebook with data analysis and model results |
| `Predicting Initiating Events in Narrative Texts.pdf` | PDF export of the main notebook |
| `UnitTest3.ipynb` | Alternate version of the analysis used during testing |
| `key_features_importance.md` | Explanation of top linguistic features (optional summary) |
| `data/` | Narrative dataset and derived features |

---

## Conclusion

This project demonstrates how machine learning can support the analysis of narrative writing by identifying patterns linked to storytelling quality.  
Although the model's accuracy is moderate, it highlights measurable aspects of language and structure that contribute to effective storytelling.  
With further refinement and more data, such models could assist educators in assessing narrative development more efficiently and consistently.