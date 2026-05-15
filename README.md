# NyayaSaar-LoRA

NyayaSaar-LoRA is a lightweight PEFT/QLoRA-based legal AI project focused on simplifying structured Indian legal reasoning into plain English.

The project explores whether small language models can improve legal accessibility while preserving core reasoning structure using IRAC-style representations.

---

## Motivation

Indian legal documents are often difficult for ordinary citizens to understand because of:

* archaic legal terminology,
* procedural complexity,
* long sentence structures,
* and formal legal drafting styles.

This project investigates whether parameter-efficient fine-tuning (LoRA/QLoRA) can help small language models simplify legal reasoning while preserving meaning.

The focus is on:

* accessibility,
* explainability,
* low-resource adaptation,
* and socially useful legal AI.

---

## Example

### Input

```text
Issue: Whether the detention order violates Article 22.

Rule: Preventive detention laws require procedural safeguards.

Application: The petitioner argued safeguards were not followed.

Conclusion: The detention order is quashed.
```

### Simplified Output

```text id="qspqaz"
The court examined whether the detention was legal under the Constitution.

The law says preventive detention must follow proper safeguards.

The petitioner argued these safeguards were ignored.

The court agreed and cancelled the detention order.
```

---

## Technical Stack

* Qwen2.5-0.5B-Instruct
* LoRA / QLoRA
* PEFT
* Unsloth
* Hugging Face Transformers
* Google Colab

---

## Dataset

This project uses the inIRAC dataset:

🔗 Dataset:
https://huggingface.co/datasets/joyboseroy/inIRAC

The dataset structures Indian legal reasoning into:

* Issue
* Rule
* Application
* Conclusion

---

## Model

🔗 Hugging Face Model:
https://huggingface.co/joyboseroy/nyayasaar-lora

---

## Research Context

This project complements the following research work:

**Falkor-IRAC: Graph-Constrained Generation for Verified Legal Reasoning in Indian Judicial AI**

https://arxiv.org/abs/2605.14665

---

## Running the Notebook

Open the notebook in Google Colab and run all cells.

### Install dependencies

```bash
pip install unsloth transformers datasets peft trl accelerate bitsandbytes textstat
```

---

## Project Goals

* Simplify legal reasoning for non-lawyers
* Explore low-resource legal NLP
* Investigate structured legal abstraction
* Improve accessibility in Indian Legal AI

---

## Limitations

This project is a research prototype and:

* does not provide legal advice,
* may oversimplify legal nuances,
* and should not be used in high-stakes legal settings.

Outputs should always be reviewed by qualified legal professionals.

---

## Future Work

Potential future directions include:

* multilingual legal simplification,
* Hindi/Bengali adaptation,
* readability evaluation metrics,
* graph-grounded legal reasoning,
* and retrieval-augmented explanation systems.

---

## Author

Joy Bose

Senior Data Scientist and Researcher

Research interests:

* Legal AI
* Explainable AI
* Graph Reasoning
* Ethical AI
* Efficient LLM Adaptation
